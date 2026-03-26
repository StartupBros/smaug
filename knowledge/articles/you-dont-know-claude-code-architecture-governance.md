---
title: "You Don't Know Claude Code: Architecture, Governance, and Engineering Practices"
type: article
date_added: 2026-03-17
source: "https://x.com/i/article/2032364186022686720"
author: "Tw93 (HiTw93)"
tags: []
via: "Twitter bookmark from @HiTw93"
---

A deeply practical handbook for engineers who want more predictable, controllable, and verifiable workflows from Claude Code. Written by Tw93 (creator of the Kaku terminal) based on six months of heavy use and ~$40/month across two accounts, originally published in Chinese to 6,000+ likes, then translated to English. The core thesis: most Claude Code failures are systems-design problems, not prompting problems. The author frames Claude Code as a six-layer system — Execution Model, Concept Boundaries, Context Engineering, Skills Design, Tool Design, and Hooks — and argues that over-indexing on any single layer destabilizes the whole system.

The article covers context management in unusual depth: MCP server tool definitions alone can consume 25K+ tokens of fixed overhead, and the default compression algorithm tends to silently discard architectural decisions first. The author recommends explicit Compact Instructions in CLAUDE.md to control what survives compression, plus a HANDOFF.md pattern for cross-session continuity. On Skills design, the key insight is that skill descriptors stay permanently in context while bodies load on demand — so verbose descriptors are expensive at every turn. On verification: "if you can't clearly explain how Claude knows it's done correctly, the task probably isn't suitable for autonomous completion." The article closes with a full reference directory layout and a health-check skill (`tw93/claude-health`) that evaluates a project's Claude Code configuration against these principles.

## Key Takeaways

- Claude Code is a systems-design problem, not a prompting problem — treat it as a six-layer architecture
- MCP server definitions can silently consume 12.5%+ of your context budget before any task starts
- The default compaction algorithm removes architectural decisions first; use Compact Instructions to override
- Skills: keep descriptors under ~10 tokens; long descriptors pollute every turn of every session
- Hooks are for deterministic enforcement (formatting, protected-file guards, notifications) — not semantic judgment
- Subagents are primarily for isolation, not parallelism; grant them narrower permissions than the main thread
- Prompt caching is architecture: stable prefix ordering (system → tools → history → input) is a first-class design constraint
- Switching models mid-session invalidates the entire cache for the new model — use subagent handoffs instead
- The verification loop is non-negotiable: define acceptance criteria upfront or the task isn't ready for autonomous execution
- CLAUDE.md is a collaboration contract, not documentation; start empty and add only what must hold across every session

## Links

- [Article](https://x.com/i/article/2032364186022686720)
- [tw93/claude-health on GitHub](https://github.com/tw93/claude-health)
- [Kaku terminal project](https://github.com/tw93/Kaku)
- [Original Tweet](https://x.com/HiTw93/status/2033911478466843115)
