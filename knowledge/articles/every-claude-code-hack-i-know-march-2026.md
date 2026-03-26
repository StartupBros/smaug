---
title: "Every Claude Code Hack I Know (March 2026)"
type: article
date_added: 2026-03-22
source: "https://x.com/i/article/2035834194065281024"
author: "mvanhorn"
tags: [claude-code, workflow, productivity, agentic-coding, compound-engineering]
via: "Twitter bookmark from @kevinrose"
---

A practitioner's account of a fully voice-driven, parallel-session Claude Code workflow built around plan.md files rather than an IDE. The author (@mvanhorn, #3 contributor to Compound Engineering) describes running 4–6 simultaneous Ghostty sessions with Zed autosave as the live editing surface — each session handling a different plan, task, or bug in parallel. Voice dictation via Monologue pipes speech directly into the focused app, eliminating typing entirely.

The core loop is: research with `/last30days`, generate a structured `plan.md` with `/ce:plan`, then execute with `/ce:work`. Plans survive context window resets and act as checkpoints for subagent delegation. The article walks through `skipDangerousModePermissionPrompt`, Stop hooks for audio notifications, and 500ms Zed autosave to enable fully autonomous parallel operation. It also covers using a Mac Mini + tmux for remote sessions (airplane-proof) and Telegram integration for phone-to-agent messaging.

The Disney World example illustrates the workflow applied to non-code tasks: `/last30days` research → `/ce:plan` itinerary → Vercel deploy → OpenClaw cron reminders, all done from a soccer field sideline.

## Key Takeaways

- Replace IDE-centric thinking with plan.md files: every task starts with `/ce:plan`, even one-liners get a plan unless truly trivial
- Run 4–6 parallel Claude Code sessions; `skipDangerousModePermissionPrompt: true` is mandatory for async context-switching
- `/last30days` (open source, 4.5K stars) searches Reddit/X/YouTube/HN in parallel before planning — grounds plans in current community knowledge, not stale training data
- Stop hooks + `afplay` sound notification let you walk away and return when a session finishes
- Zed `autosave` at 500ms + Claude Code filesystem watching creates a Google-Docs-like live co-editing experience
- Mac Mini + tmux makes Claude sessions airplane/disconnect-proof; Telegram integration enables phone-to-agent task dispatch
- When token budgets run out, `/ce:work --codex` delegates implementation to OpenAI Codex credits as a complementary resource

## Links

- [Article](https://x.com/i/article/2035834194065281024)
- [Original Tweet](https://x.com/kevinrose/status/2035895141026922684)
- [last30days on GitHub](https://github.com/mvanhorn/last30days-skill)
- [Compound Engineering Plugin](https://github.com/EveryInc/compound-engineering-plugin)
