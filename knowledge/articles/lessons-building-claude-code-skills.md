---
title: "Lessons from Building Claude Code: How We Use Skills"
type: article
date_added: 2026-03-17
source: "https://x.com/i/article/2033772621536591872"
author: "Thariq Shihipar (trq212)"
tags: []
via: "Twitter bookmark from @trq212"
---

An in-depth article from someone at Anthropic sharing lessons learned from running hundreds of Claude Code skills internally. The key insight is that skills are folders, not just markdown files — the filesystem itself is a context engineering and progressive disclosure mechanism. The article catalogs nine recurring skill types (Library & API Reference, Product Verification, Data Fetching, Business Process Automation, Code Scaffolding, Code Quality, CI/CD, Runbooks, Infrastructure Operations) and then gives detailed practical guidance on skill authorship: avoiding stating the obvious, building a Gotchas section from observed failure points, using the file system for progressive disclosure, avoiding over-specifying instructions, storing setup in config.json, writing descriptions for the model (not humans), using memory via append-only logs or SQLite, embedding scripts so Claude composes rather than reconstructs, and using on-demand hooks that only activate when a skill is invoked. Distribution advice covers repo-checked skills vs. internal plugin marketplaces, organic curation before marketplace promotion, and skill composition by name reference.

## Key Takeaways

- Skills are folders that can contain scripts, assets, templates, and data — treat the whole filesystem as context engineering
- Nine skill types cataloged: library reference, product verification, data fetching, business process, scaffolding, code quality, CI/CD, runbooks, infrastructure ops
- Gotchas section is the highest-signal content in any skill; build it from observed Claude failure points over time
- The `description` field is scanned by the model to decide when to trigger the skill — write it for the model, not the human
- On-demand hooks last for the session only, enabling opinionated guardrails (e.g., block `rm -rf`) without always-on annoyance
- At scale, use an internal plugin marketplace with organic traction-based curation rather than checking all skills into repos
- Memory within a skill (standups.log, SQLite) lets Claude build on its own history across sessions

## Links

- [Article](https://x.com/i/article/2033772621536591872)
- [Original Tweet](https://x.com/trq212/status/2033949937936085378)
