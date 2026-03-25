---
title: "Anatomy of the .claude/ Folder"
type: article
date_added: 2026-03-22
source: "https://x.com/i/article/2034961967149195264"
author: "Akshay Pachaar"
tags: [claude-code, configuration, developer-tools, ai-agents]
via: "Twitter bookmark from @iruletheworldmo"
---

A comprehensive guide to every file and folder in the .claude/ directory, explaining how Claude Code's configuration system works. Covers CLAUDE.md (the primary instruction file), settings.json (permissions and tool access), commands/ (custom slash commands), rules/ (modular path-scoped instructions), skills/ (auto-invoked workflows), and agents/ (specialized subagent personas). Also covers the global ~/.claude/ folder for personal preferences.

Key insight: there are actually two .claude directories — one project-level (committed to git, shared with team) and one global at ~/.claude/ (personal preferences across all projects).

## Key Takeaways

- CLAUDE.md is the highest-leverage file: keep it under 200 lines, focus on build commands, architecture decisions, and non-obvious gotchas
- CLAUDE.local.md and settings.local.json are auto-gitignored for personal overrides
- rules/ folder enables modular, path-scoped instructions that scale better than one giant CLAUDE.md
- commands/ files become /project:command-name slash commands; files in ~/.claude/commands/ become /user:command-name
- skills/ auto-invoke when the task description matches; commands wait for explicit invocation
- agents/ define specialized subagent personas with restricted tools and preferred models
- settings.json allow/deny lists control which tools run without confirmation vs. blocked entirely

## Links

- [Article](https://x.com/i/article/2034961967149195264)
- [Original Tweet](https://x.com/iruletheworldmo/status/2035637459183104197)
