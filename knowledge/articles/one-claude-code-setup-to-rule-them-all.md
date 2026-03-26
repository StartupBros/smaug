---
title: "One Claude Code Setup to Rule Them All"
type: article
date_added: 2026-03-25
source: "https://x.com/i/article/2036476761920126976"
author: "Griffin Hilly"
tags: [claude-code, claude-md, workflow, productivity, agent-orchestration, bookmarks]
via: "Twitter bookmark from @RoundtableSpace"
---

Griffin Hilly distilled hundreds of Claude Code workflow posts (including community tips from Karpathy, doodlestein, synopsi, and others) into a single opinionated setup published as a GitHub repo (`griffinhilly/claude-code-synthesis`). The core claim: most people's CLAUDE.md files are bloated, contradictory, and fighting themselves — a single well-structured global config file changes every session. He also describes a bookmark pipeline that turns saved Twitter posts into a semantic-searchable knowledge base using HAR file extraction and embeddings.

The setup centers on a "COMP" system per project (CLAUDE.md for AI behavior, ORIENT.md for human onboarding, MEMORY.md for accumulated decisions, PLAN.md for roadmap) and a set of situational guides Claude loads on-demand rather than keeping everything in one long file. Key doctrine points include Orchestrator-First (the session agent manages and delegates, never does direct work), Dialectic Reviews (spawn opposing FOR/AGAINST agents with a referee instead of asking one agent for pros/cons), and Evals-Before-Specs (define success criteria before writing the spec).

The meta-move described is using Claude itself to read your bookmarks weekly and incorporate anything new. The article synthesizes a community of practice around Claude Code configuration into one actionable starting point, citing specific contributors for each principle.

## Key Takeaways

- CLAUDE.md should encode a "Leverage Doctrine" (you ideate/decide, Claude researches/executes) and use trigger rules to load guides on-demand rather than dumping everything upfront
- Orchestrator-First pattern: session agent decides whether to handle directly, delegate to subagent, or route to MCP — never acts as both planner and worker
- Dialectic Reviews (Hunter/Skeptic/Referee) outperform asking a single agent for pros and cons of a decision
- COMP system separates AI behavior, human orientation, accumulated knowledge, and direction into four distinct files per project
- The bookmark pipeline (HAR extraction → categorization → embeddings → semantic search) turns curated Twitter saves into a queryable knowledge base

## Links

- [Article](https://x.com/i/article/2036476761920126976)
- [GitHub repo](https://github.com/griffinhilly/claude-code-synthesis)
- [Original Tweet](https://x.com/GriffinHilly/status/2036518973546598508)
