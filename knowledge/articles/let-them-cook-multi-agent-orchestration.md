---
title: "Let Them Cook: Lessons from 6 Weeks of Multi-Agent Orchestration"
type: article
date_added: 2026-02-04
source: "https://x.com/i/article/2019011014855884800"
author: "Khaliq Gant"
tags: []
via: "Twitter bookmark from @Khaliqgant"
---

Six weeks of building Agent Relay (an open-source CLI-agnostic communication layer for multi-agent AI workflows) using Agent Relay itself. The author reports 4–5x speed improvements and increased code quality when running coordinated agent swarms, but also documents significant failure modes.

The core insight is that different CLI agents have fundamentally different communication styles that should drive staffing decisions: Claude communicates well and can be interrupted, making it ideal for Lead and Reviewer roles; Codex does heads-down work but goes dark and is hard to interrupt, making it better for isolated implementation tasks; Cursor is fast with tight feedback loops. The "magic ratio" of Lead-to-worker agents is 2–5 workers per Lead — larger swarms overwhelm the Lead and cause it to enter infinite loops and die. Agent laziness (stubbing implementations with TODOs) compounds in swarms and requires shadow agents plus reviewer agents to catch. The continuity concept (agents saving trajectory state in structured JSON chapters) is highlighted as an unexpected unlock — future agents can pick up prior context instantly rather than starting cold.

## Key Takeaways

- 2–5 worker agents per Lead is the practical sweet spot; 10+ agents per Lead causes failure
- Staff by communication style: Claude for Lead/Reviewer, Codex for deep isolated implementation, Cursor for rapid iteration
- Agent laziness (incomplete stubs reported as done) compounds across swarms — shadow agents and reviewer agents are essential mitigations
- Trajectory storage (structured JSON logs of agent reasoning by chapter) dramatically accelerates context recovery in new sessions
- The planning phase becomes the critical human bottleneck — vague specs cause agents to cut corners at scale
- Agent Relay is CLI-agnostic and open source, with a `teams.json` config for codifying team composition and auto-spawn on session start

## Links

- [Article](https://x.com/i/article/2019011014855884800)
- [GitHub: AgentWorkforce/relay](https://github.com/AgentWorkforce/relay)
- [Original Tweet](https://x.com/Khaliqgant/status/2019124627860050109)
