---
title: "Anatomy of the .claude/ folder"
type: article
date_added: 2026-03-22
source: "https://x.com/i/article/2034961967149195264"
author: "akshay_pachaar"
tags: [claude-code, configuration, workflow, developer-tools]
via: "Twitter bookmark from @iruletheworldmo"
---

A complete guide to CLAUDE.md, custom commands, skills, agents, and permissions inside the `.claude/` folder — the control center for how Claude Code behaves in a project.

The article draws a key distinction: there are two `.claude/` directories. The project-level one gets committed to git and shared with the team (rules, commands, agents, permissions). The global `~/.claude/` holds personal preferences, session history, and auto-memory. CLAUDE.md is the highest-leverage file — loaded directly into the system prompt at session start. Keep it under 200 lines; longer files cause instruction-following degradation.

The `.claude/rules/` folder enables modular, path-scoped instructions: files with YAML frontmatter `paths:` fields only load when Claude is editing matching files, avoiding context bloat. Custom slash commands live in `.claude/commands/` (shared) or `~/.claude/commands/` (personal, as `/user:...`); they support `!backtick` shell injection and `$ARGUMENTS` for parameterization. Skills in `.claude/skills/` are like commands but auto-invoked by Claude when the task matches their description — they can bundle supporting files. Agents in `.claude/agents/` are specialized subagent personas with isolated context windows, restricted toolsets, and optional model selection.

## Key Takeaways

- CLAUDE.md is loaded into the system prompt on every session — keep it under 200 lines focused on commands, architecture, conventions, and non-obvious gotchas
- Use `.claude/rules/` with path-scoped frontmatter to split a crowded CLAUDE.md into maintainable, purpose-specific files
- Commands (`/project:name`) are slash-triggered, single-file; Skills are auto-invoked by Claude and can bundle multiple supporting files in a subdirectory
- Agents run in isolated context windows with restricted tool access and optional cheaper model selection — useful for focused read-only tasks
- `settings.json` `allow`/`deny` lists control which shell commands run without confirmation; anything not listed triggers a prompt
- `CLAUDE.local.md` and `settings.local.json` are auto-gitignored for personal overrides that shouldn't land in the repo

## Links

- [Article](https://x.com/i/article/2034961967149195264)
- [Original Tweet](https://x.com/iruletheworldmo/status/2035637459183104197)
