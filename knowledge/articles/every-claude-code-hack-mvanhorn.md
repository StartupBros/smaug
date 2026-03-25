---
title: "Every Claude Code Hack I Know (March 2026)"
type: article
date_added: 2026-03-22
source: "https://x.com/i/article/2035834194065281024"
author: "Matt Van Horn (@mvanhorn)"
tags: [claude-code, developer-tools, workflow, ai-agents, productivity]
via: "Twitter bookmark from @kevinrose"
---

A practical guide from Matt Van Horn covering his complete Claude Code workflow as of March 2026. Written from the perspective of someone who has 70 plan files and 263 commits in 30 days. Core philosophy: "No IDE. Just plan.md files and voice."

Uses Compound Engineering plugin (/ce:plan, /ce:work, /last30days), Monologue for voice input, Zed with 500ms autosave, and Ghostty terminal. Runs 4-6 parallel Claude Code sessions simultaneously.

## Key Takeaways

- /ce:plan is the entry point for everything: ideas, bugs, errors (paste screenshots directly), new features — always plan before coding
- /last30days runs parallel research across Reddit, X, YouTube, HN before planning, grounding plans in current community knowledge
- Three critical settings: dangerouslySkipPermissions, skipDangerousModePermissionPrompt, and Zed 500ms autosave
- 4-6 parallel Ghostty windows each running separate Claude sessions — while one plans, another builds, another researches
- plan.md files are checkpoints that survive context loss: start new session, point at plan, continue
- Mac Mini + tmux for remote sessions: laptop closes on airplane, session keeps running on the machine
- Granola meeting transcripts + codebase context + prior strategy plans = one-shot product proposals
- /ce:work --codex delegates implementation to Codex when Claude credits run low
- Sound hook on Stop event signals when a session completes so you can context-switch efficiently
- Contributors: @danshapiro tip on bypass permissions, Myk Melez on sound hook, Nathan Smith on tmux airplane trick

## Links

- [Article](https://x.com/i/article/2035834194065281024)
- [last30days GitHub](https://github.com/mvanhorn/last30days-skill)
- [Original Tweet](https://x.com/kevinrose/status/2035895141026922684)
