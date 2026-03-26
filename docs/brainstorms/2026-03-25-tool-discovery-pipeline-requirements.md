---
date: 2026-03-25
topic: tool-discovery-pipeline
---

# Tool Discovery Pipeline

## Problem Frame

Smaug already discovers tools via bookmarks and files them to `knowledge/tools/`, but there's no path from "interesting GitHub repo someone tweeted" to "tested recommendation in the House of Vibe vault." Today, creating a vault resource means manually re-researching a tool you already bookmarked weeks ago. The discovery data is there; the editorial layer and publishing pipeline are not.

The vault should contain authentic recommendations backed by real usage, not auto-generated listicles. This requires a human editorial gate between discovery and publication.

## Requirements

- R1. **Auto-annotate on discovery.** When `process-bookmarks` files a GitHub repo to `knowledge/tools/`, automatically create a `discovered` entry in `data/tools/annotations.yaml` linking to the knowledge file.
- R2. **Annotations sidecar.** `data/tools/annotations.yaml` tracks each tool's evaluation status and editorial metadata. Each entry references its knowledge file and records: status, dates, who shared it (`via` fields from knowledge file and any additional sharers), and editorial fields (take, use_case, difficulty) populated when vault-worthy.
- R3. **Status lifecycle.** Each tool follows: `discovered` -> `trying` | `skip`, then `trying` -> `vault-worthy` | `skip`. Status transitions are recorded with dates.
- R4. **Curation command.** `/curate-vault-tools` surfaces tools that need attention. Shows a batch summary table sorted by signal strength: multiple sharers > star count > recency. From the table, you drill into individual tools to review and set status.
- R5. **Trying nudge.** Tools with status `trying` appear in a separate "Currently Trying" section at the top of the curation view, reminding you to evaluate them.
- R6. **Editorial input on vault-worthy.** When marking a tool `vault-worthy`, the command collects: a one-liner take (your authentic opinion), a House of Vibe use case (who it's for / when to use it), and a difficulty level (beginner / intermediate / advanced).
- R7. **Vault resource generation.** When a tool is marked vault-worthy, generate a vault markdown file combining Smaug's knowledge file (description, features, links) with your editorial annotation (take, use case, difficulty). The resource maps to `resource_type: 'tool'` in the vault schema.
- R8. **Direct write to prbot.** The generated vault file is written directly to `~/SITES/prbot/apps/startupbros/content/vault/`. The user commits and syncs in prbot separately.
- R9. **Inbox compounding.** Tools marked `skip` never resurface. Tools marked `vault-worthy` are excluded from the discovery inbox. Only `discovered` and `trying` tools appear during curation. The annotations file becomes a durable record of the evaluation process.

## Success Criteria

- Running `/curate-vault-tools` surfaces recently discovered tools with enough context (README summary, star count, who shared it) to make a try/skip decision in seconds.
- Going from "I've used this tool and like it" to "vault resource published" takes under 2 minutes of editorial input.
- The vault never contains a tool you haven't actually used and endorsed.

## Scope Boundaries

- **Tools only.** Articles, videos, and podcasts are out of scope. The pattern can extend to those later.
- **No auto-publishing.** The pipeline ends at writing the vault markdown file. Content-sync and Supabase publishing are existing prbot concerns.
- **No GitHub API integration for star counts in this iteration.** Star count can be fetched live during curation or extracted from README content. Planning should determine the lightest approach.
- **No retroactive backfill.** Existing `knowledge/tools/` files don't automatically get annotations. They can be manually added or a one-time backfill script can be a follow-up.

## Key Decisions

- **Batch table over one-at-a-time:** Most discovered tools will be skipped. A scannable table lets you skip fast; signal-based sort order (from option 3) is baked into the sort rather than being a filter.
- **Take + use case + difficulty:** Enough editorial voice to feel authentic without being a friction bottleneck. Difficulty maps directly to the vault's existing schema field.
- **Direct cross-repo write:** Same pattern as other Smaug -> prbot output steps. Smaug writes the file; prbot handles sync.
- **Annotations in Smaug, not in knowledge files:** The knowledge file stays a clean research artifact. Editorial state lives in the sidecar. This mirrors the X Creator Directory pattern.

## Dependencies / Assumptions

- `process-bookmarks` command continues to file GitHub repos to `knowledge/tools/` (existing behavior, no change needed to the filing logic itself).
- `~/SITES/prbot/apps/startupbros/content/vault/` is the correct output path and the content-sync pipeline will pick up new `.md` files there.
- The vault's `VaultFrontmatterSchema` (title, slug, description, resource_type, tags, difficulty, etc.) is stable.

## Outstanding Questions

### Deferred to Planning

- [Affects R4][Needs research] What's the lightest way to get GitHub star counts during curation? Options: live GitHub API call, scrape from README content, or store in annotation at discovery time.
- [Affects R1][Technical] Exact integration point in `process-bookmarks` — should the annotation write happen in the main command logic, in a post-processing hook, or as a separate step?
- [Affects R7][Technical] Vault resource markdown template — exact frontmatter fields and body structure should be derived from existing vault content patterns and the `VaultFrontmatterSchema`.
- [Affects R2][Technical] Annotation schema design — exact YAML structure for entries (keyed by slug? by source URL?).

## Next Steps

-> `/ce:plan` for structured implementation planning
