---
title: "ralph"
type: tool
date_added: 2026-01-21
source: "https://github.com/snark-tank/ralph"
tags: []
via: "Twitter bookmark from @aakashgupta"
---

Ralph is a bash loop that runs an AI coding agent (Claude Code) repeatedly and autonomously until a list of tasks is complete. Named after the Simpsons character known for naive, relentless persistence, it breaks work into atomic tasks with binary success criteria, processes them one at a time with clean context each round, and commits progress incrementally via git. Designed by Geoffrey Huntley, it enables "AFK coding" — setting an agent loop running overnight and waking to finished features.

## Key Features

- Loop-based autonomous task execution with configurable round limits (e.g. 10–20 rounds)
- Clean context per round — no accumulated confusion from previous iterations
- Progress persistence via git commits, a progress file, and a task list
- Binary pass/fail success criteria so the agent knows when a task is done without asking
- Compounding knowledge: each round logs what it learned; next round reads those logs
- Typical cost ~$30 per 10-round run vs. $400–600/day for a senior dev

## Links

- [GitHub](https://github.com/snark-tank/ralph)
- [Original Tweet](https://x.com/aakashgupta/status/2013850023688315172)
