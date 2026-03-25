---
title: "My chief of staff, Claude Code"
type: article
date_added: 2026-03-05
source: "https://x.com/i/article/2029698920159531010"
author: "Jim Prosser"
tags: [claude-code, automation, productivity, ai-agents, personal-assistant]
via: "Twitter bookmark from @jimprosser"
---

Jim Prosser (non-programmer, solo tech communications consultant) describes building a fully automated personal operations system in 36 hours using Claude Code. The system runs on a Mac Studio and handles morning triage, parallel task dispatch, and calendar time-blocking.

## Key Takeaways

- **Overnight automation**: Two cron-like processes run before he wakes — one calculates real Google Maps drive times for calendar events, another triages email and creates Todoist tasks with priorities and duration estimates
- **AM Sweep (Stream Deck button)**: Claude Code classifies all tasks into Green (dispatch fully), Yellow (prep 80%), Red (human required), Gray (defer) — then six parallel subagents handle email drafting, Obsidian notes, scheduling, and research simultaneously
- **Time Block (second button)**: Turns remaining tasks into a time-blocked calendar with geo-batched errands, gym scheduling, and load-aware future deferral — takes about one minute
- **Architecture insight**: Each layer feeds metadata to the next — the email scanner attributes tasks so the AM Sweep can classify them; the AM Sweep packages context for subagents; the time-blocker reads upstream output. Systems thinking, not software engineering
- **Human boundaries**: Never sends email (only drafts), never writes strategic documents, never makes pricing or relationship decisions. Bias toward "prep" on ambiguous tasks
- **Cost**: ~$5-10/month beyond the $100/month Claude Max plan; replaces $400-1,000/month for a part-time VA; saves 130-195 hours/year on morning operations alone

## Links

- [Article](https://x.com/i/article/2029698920159531010)
- [Original Tweet](https://x.com/jimprosser/status/2029699731539255640)
