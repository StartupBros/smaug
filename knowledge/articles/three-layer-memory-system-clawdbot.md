---
title: "The Three-Layer Memory System Upgrade for Clawdbot"
type: article
date_added: 2026-01-27
source: "https://x.com/i/article/2015965409682587648"
author: "pixel (@spacepixel)"
tags: []
via: "Twitter bookmark from @spacepixel"
---

A detailed implementation guide for upgrading Claude's (Clawdbot's) default static memory into a self-maintaining, compounding knowledge graph. The system replaces manually-maintained flat files with three coordinated layers: a structured knowledge graph of entities, daily event logs, and a tacit preferences file. The key insight is that memory should supersede stale facts rather than delete them, preserving full history while keeping active context current through weekly automated synthesis.

## Key Takeaways

- **Layer 1 — Knowledge Graph** (`/life/areas/`): Entity folders for people, companies, projects, each with `summary.md` (weekly-rewritten snapshot) and `items.json` (atomic timestamped facts). Facts are never deleted — contradicted ones get `status: "superseded"` with a pointer to the replacement.
- **Layer 2 — Daily Notes** (`memory/YYYY-MM-DD.md`): Raw event log capturing what happened and when; a cheap sub-agent (e.g. Haiku) scans these every ~30 minutes to extract durable facts into Layer 1.
- **Layer 3 — Tacit Knowledge** (`MEMORY.md`): Patterns, preferences, and lessons about how you operate — distinct from facts about the world.
- **Compounding engine**: Real-time extraction runs on a heartbeat (~$0.001/run), weekly Sunday cron rewrites summaries and prunes stale context automatically — no manual edits needed.
- **Why it beats RAG**: All human-readable and searchable flat files vs. black-box vector databases; scales indefinitely without context window bloat because summaries stay lean.
- Implementation requires adding directives to `AGENTS.md` and `HEARTBEAT.md`, plus a weekly synthesis cron job with a defined atomic fact JSON schema.

## Links

- [Article](https://x.com/i/article/2015965409682587648)
- [Original Tweet](https://x.com/spacepixel/status/2015967798636556777)
