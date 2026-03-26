---
title: "The complete claude code tutorial"
type: article
date_added: 2026-01-10
source: "https://x.com/i/article/2010075005044867073"
author: "Eyad Khrais"
tags: []
via: "Twitter bookmark from @eyad_khrais"
---

A practitioner's guide to Claude Code written by a 7-year SWE (ex-Amazon, Disney, Capital One), now CTO of an enterprise agent startup. The article is structured around a handful of high-leverage principles: always enter plan mode (Shift+Tab twice) before typing; write a tight CLAUDE.md that is specific to the project, explains the *why* behind each rule, and gets updated continuously; respect context window degradation (quality starts slipping at 20-40% capacity, not at 100%); scope conversations to one task at a time and use external memory files (SCRATCHPAD.md, plan.md) across sessions; and prompt with constraints and examples rather than open-ended requests. The article also covers model selection (Opus for planning and complex reasoning, Sonnet for execution), use of MCP servers, hooks, and custom slash commands, and how to move from one-off interactive use to scripted/headless automation via `claude -p` for enterprise workflows.

## Key Takeaways

- Plan mode produces dramatically better output than typing directly; the author calls it a 5-minute investment that saves hours
- CLAUDE.md is the highest-leverage config file: keep it under ~150 instructions, explain the *why*, update it live with the `#` key
- Context degrades at ~20-40% usage, not 100%; use `/compact`, `/clear`, and external memory files to stay in the quality zone
- Scope one conversation per feature; "copy-paste reset" is a practical technique for preserving critical info across a fresh context
- Use Opus for planning and architecture decisions, switch to Sonnet for implementation to balance cost and quality
- Claude's `--headless` (`-p`) flag enables pipeline automation: PR reviews, ticket triage, documentation updates
- The improvement flywheel: Claude makes a mistake → review logs → improve CLAUDE.md → Claude gets better

## Links

- [Article](https://x.com/i/article/2010075005044867073)
- [Original Tweet](https://x.com/eyad_khrais/status/2010076957938188661)
