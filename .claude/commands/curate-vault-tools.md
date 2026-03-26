# /curate-vault-tools

Surface recently discovered tools for editorial review and publish vault-worthy ones to the House of Vibe.

## Before You Start

### CRITICAL: Use Edit Tool for annotations.yaml (DATA LOSS PREVENTION)

**NEVER use the Write tool on `data/tools/annotations.yaml`.** The Write tool REPLACES the entire file.

**ALWAYS use the Edit tool** to update annotation entries. The Edit tool preserves existing content while making targeted changes.

### CRITICAL: Check vault output directory early

Before collecting any editorial input, verify the vault output directory exists:
```bash
VAULT_DIR=$(node -e "const c=require('./smaug.config.json'); const os=require('os'); const p=c.vaultOutputDir||'~/SITES/prbot/apps/startupbros/content/vault'; console.log(p.replace(/^~/, os.homedir()))")
[ -d "$VAULT_DIR" ] && echo "OK: $VAULT_DIR" || echo "MISSING: $VAULT_DIR — vault writes will fail"
```

If missing, warn the user immediately and ask whether to continue (status changes still work, only vault file generation needs the directory).

## Setup

**Get today's date:**
```bash
date +"%Y-%m-%d"
```

**Load config paths:**
```bash
node -e "const c=require('./smaug.config.json'); console.log(JSON.stringify({annotationsFile:c.annotationsFile||'./data/tools/annotations.yaml', vaultOutputDir:c.vaultOutputDir||'~/SITES/prbot/apps/startupbros/content/vault'}, null, 2))"
```

**Read annotations file:**
Read `data/tools/annotations.yaml` (or path from config). If the file fails to parse:
- Warn the user: "annotations.yaml appears malformed"
- Offer to back up the file and recreate from the schema template
- Do NOT silently continue with bad data

**Filter to actionable tools:**
- `trying` status tools → "Currently Trying" section
- `discovered` status tools → batch discovery table
- `skip` and `vault-worthy` tools → excluded entirely (inbox compounding)

If no actionable tools exist, report "No tools to review — all discovered tools have been evaluated" and exit.

**Read knowledge files for context:**
For each actionable tool, read its `knowledge_file` path to extract the first paragraph (description) for the table display. If a knowledge file is missing:
- Show the tool with `[knowledge file missing]` instead of a description
- The tool is still reviewable using annotation metadata (source URL, stars, sharers)

## Phase 1: Currently Trying (Nudge)

If any tools have `status: trying`, present them first:

```
## Currently Trying

You've been trying these tools. Ready to evaluate any?

| # | Tool | Trying Since | Days | Source |
|---|------|-------------|------|--------|
| T1 | {title} | {trying_date} | {days} | {source_url} |
```

For each trying tool, show:
- Tool name (from knowledge file title or slug)
- Date marked as trying
- Days since trying date (calculated from today)
- Source URL (GitHub link)

Ask: "Enter a number to evaluate (e.g., T1), or press Enter to skip to new discoveries."

For tools selected from trying:
- `vault-worthy` → enter editorial input flow (see Phase 4)
- `skip` → set `status: skip`, `skipped: {today}`

## Phase 2: Batch Discovery Table

Present `discovered` tools sorted by signal strength:

**Sort order (highest signal first):**
1. Multiple sharers (`via` array length > 1)
2. Star count (descending)
3. Recency (discovered date, newest first)

```
## Recently Discovered Tools

| # | Tool | Stars | Sharers | Discovered | Description |
|---|------|-------|---------|------------|-------------|
| 1 | {title} | {stars} | {via_count} | {date} | {one_line_description} |
| 2 | {title} | {stars} | {via_count} | {date} | {one_line_description} |
```

**Columns:**
- `#`: Row number for selection
- `Tool`: Name from knowledge file title (or slug if knowledge file missing)
- `Stars`: GitHub star count from annotation
- `Sharers`: Count of unique sharers in `via` array (show handles if 2-3, just count if more)
- `Discovered`: Date in YYYY-MM-DD format
- `Description`: First sentence from knowledge file, truncated to ~80 chars

## Phase 3: Collect Decisions

After presenting the table, prompt for decisions:

```
Actions: skip, try, vault-worthy, open
Enter decisions (e.g., "skip 1,3,5" or "try 2" or "open 4" or "vault-worthy 6"):
```

**Supported input formats:**
- `skip 1,3,5,7` — bulk skip multiple tools
- `skip all` — skip all remaining discovered tools
- `try 2` — mark tool #2 as trying
- `vault-worthy 4` — enter editorial input flow for tool #4
- `open 3` — show full knowledge file content for tool #3, then return to prompt
- Individual number (e.g., `4`) — show that tool's details and ask for action

**Status transitions:**
- `skip` → set `status: skip`, `skipped: {today}`. Never resurfaces.
- `try` → set `status: trying`, `trying: {today}`. Appears in trying nudge next run.
- `vault-worthy` → proceed to Phase 4 (editorial input)

After processing a batch of decisions, ask: "Continue reviewing, or stop here?"
- If continuing, show remaining undecided tools
- If stopping, proceed to Phase 5 (write changes)

## Phase 4: Vault-Worthy Editorial Input

When a tool is marked `vault-worthy`, collect editorial input before generating the vault file.

**Prompt for three fields:**

1. **Take** — "What's your one-liner take on {tool_name}?"
   - Free text, the user's authentic opinion
   - Example: "The fastest way to get real-time transcription running locally"

2. **Use case** — "Who is this for and when should they use it?"
   - House of Vibe audience framing
   - Example: "Solo developers who need live transcription without cloud APIs"

3. **Difficulty** — "Difficulty level? (beginner / intermediate / advanced)"
   - Must be one of: `beginner`, `intermediate`, `advanced`

**Update annotation:**
- Set `status: vault-worthy`, `vault_worthy: {today}`
- Set `take`, `use_case`, `difficulty` fields

**Generate vault markdown file:**

Read the knowledge file (`knowledge/tools/{slug}.md`) to get:
- `title` from frontmatter
- Description and key features from body
- `tags` from frontmatter
- `source` URL from frontmatter

Combine with editorial input to create the vault file:

```yaml
---
title: '{title}'
slug: {slug}
description: '{take_or_description}'
resource_type: tool
entitlement: house-of-vibe
tags:
  - Tools
  {additional_tags_from_knowledge_file}
is_featured: false
is_start_here: false
difficulty: {difficulty}
---
```

**Body structure (follow existing vault pattern):**

```markdown
## What It Does

{Description from knowledge file. Weave in the user's take naturally — don't add a separate "Our Take" callout.}

{Key features as bullet points from knowledge file}

## Who It's For

{Editorial use_case — who should use this and when}

## Getting Started

- [GitHub]({github_url})
{additional links from knowledge file if available}
```

**Write the vault file:**
```bash
# Expand vault output dir
VAULT_DIR=$(node -e "const c=require('./smaug.config.json'); const os=require('os'); const p=c.vaultOutputDir||'~/SITES/prbot/apps/startupbros/content/vault'; console.log(p.replace(/^~/, os.homedir()))")
```

Write to `{VAULT_DIR}/{slug}.md` using the Write tool (this is a new file, not an edit).

Report: "Vault file written to {path}. Remember to commit in prbot separately."

Then return to the decision prompt for remaining tools.

## Phase 5: Write All Changes

After all decisions are collected (or the user stops):

**Update `data/tools/annotations.yaml`** using the Edit tool for each changed entry:
- For `skip`: add `skipped: {today}`, change `status: skip`
- For `try`: add `trying: {today}`, change `status: trying`
- For `vault-worthy`: add `vault_worthy: {today}`, change `status: vault-worthy`, add `take`, `use_case`, `difficulty`

**CRITICAL:** Use the Edit tool for each update. Never rewrite the entire file.

**Stage and prompt for commit:**
```bash
git add data/tools/annotations.yaml
```

Ask: "Commit annotation changes? (The vault files in prbot need to be committed separately there.)"

If yes:
```bash
git commit -m "chore: curate tool annotations ({N} reviewed, {skipped} skipped, {trying} trying, {vault} vault-worthy)

Co-Authored-By: Claude Opus 4.6 <noreply@anthropic.com>"
```

## Phase 6: Report

```
Curation complete:
- {N} tools reviewed
- {skipped} skipped
- {trying} marked as trying
- {vault} published to vault

{If vault files were written:}
Vault files written to {vault_dir}:
- {slug1}.md
- {slug2}.md
Remember to commit and sync in prbot.
```
