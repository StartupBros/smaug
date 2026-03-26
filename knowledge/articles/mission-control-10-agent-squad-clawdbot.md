---
title: "The Complete Guide to Building Mission Control: How We Built an AI Agent Squad"
type: article
date_added: 2026-01-31
source: "https://x.com/i/article/2017588473751052288"
author: "Bhanu Teja P (pbteja1998)"
tags: []
via: "Twitter bookmark from @pbteja1998"
---

A comprehensive 14-part guide to building a 10-agent AI team on top of Clawdbot (now OpenClaw) for @SiteGPT. The system runs 10 named agents (Jarvis through Wong) as separate Clawdbot sessions, each with distinct roles, personalities via SOUL.md files, 15-minute heartbeat crons staggered to avoid API burst, and shared context via a Convex database called Mission Control.

The architecture: each agent is just a Clawdbot session with a specialized session key (e.g. `agent:seo-analyst:main`), a SOUL.md defining personality and domain, an AGENTS.md operating manual, and a `/memory/WORKING.md` for current task state. Agents communicate via Convex (shared task DB with comment threads, activity feed, @mention notifications, document storage) rather than direct session messaging. A daemon process polls Convex every 2 seconds and delivers @mentions to agent sessions via `clawdbot sessions send`. Thread subscriptions auto-notify agents on tasks they've touched.

Memory stack: Clawdbot JSONL session history + WORKING.md (current task) + daily notes + long-term MEMORY.md. Golden rule: if you want to remember it, write it to a file.

The 6-table Convex schema covers agents, tasks (Kanban: inbox → assigned → in_progress → review → done → blocked), messages (threaded comments), activities (event log), documents (deliverables in markdown), and notifications (@mention queue with `delivered` flag).

Lessons learned: start with 2-3 agents before scaling; use cheaper models for heartbeat/routine checks; memory requires discipline (always write to files); stagger heartbeats to prevent API bursts.

## Key Takeaways

- Each AI agent = one Clawdbot session with specialized config (SOUL.md, AGENTS.md, session key, cron schedule)
- Shared Convex database is the coordination layer—agents don't need to talk directly, they read and write shared state
- 15-minute heartbeat crons staggered at 2-minute intervals keep agents responsive without burning API credits
- Notification system queues @mentions and delivers on next heartbeat if agent is asleep
- WORKING.md is the most important memory file: agents read it first on wake to resume interrupted tasks
- Treat AI agents like team members: give roles, memory, accountability—they become a force multiplier, not just a search box

## Links

- [Article](https://x.com/i/article/2017588473751052288)
- [Original Tweet](https://x.com/pbteja1998/status/2017662163540971756)
