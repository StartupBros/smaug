---
title: "How I Use Claude Code"
type: article
date_added: 2026-01-13
source: "https://x.com/i/article/2011128658598248449"
author: "Ashpreet Bedi"
tags: []
via: "Twitter bookmark from @ashpreetbedi"
---

Ashpreet Bedi, founder of Agno (an open-source multi-agent runtime), describes building a complex "learning machines" feature entirely with Claude Code in 5 days — work that previously would have taken months. The article introduces "spec-first development": a private `specs/` repository symlinked into the codebase (gitignored, visible to Claude) where every feature gets its own folder containing CLAUDE.md (feature-level instructions), design.md (source of truth), implementation.md (progress tracker for session continuity), decisions.md (ADR-style decision log capturing the "why"), prompts.md (reusable task prompts), and future-work.md. This persists context across sessions and gives Claude structured input without relying on chat history. The article also covers layered CLAUDE.md (root level for codebase navigation + feature level for specific work), a strict PR size rule (max 5-7 files, max 500 lines, reviewable in under 10 minutes), and a "cookbooks or it didn't happen" policy where every implementation must have a runnable example script. The actual workflow: voice-transcribe a rough feature idea → Claude generates design.md → human reviews → Claude implements one small piece at a time → Claude writes cookbooks and tests → iterate → Claude updates implementation.md.

## Key Takeaways

- Spec-first development: a symlinked private `specs/` repo with per-feature folders containing design, implementation, decisions, prompts, and future-work docs — Claude writes and maintains these files
- Layered CLAUDE.md: root-level file for codebase navigation stays stable; feature-level CLAUDE.md evolves with the work
- implementation.md is the session continuity mechanism — Claude updates it so any new session can resume without reconstructing context from chat history
- decisions.md (ADR format) captures the "why" behind architectural choices, enabling future-Claude and future-human to understand reasoning
- PR discipline: enforce max 500 lines / 5-7 files in CLAUDE.md itself so Claude splits work rather than creating unmanageable diffs
- "Cookbooks or it didn't happen": every pattern needs a runnable script; if the cookbook doesn't run, implementation isn't done
- Voice transcription (whispr flow) removes the typing bottleneck for speccing features; the author barely types anymore

## Links

- [Article](https://x.com/i/article/2011128658598248449)
- [Original Tweet](https://x.com/ashpreetbedi/status/2011220028453241218)
