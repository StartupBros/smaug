---
title: "The new design process"
type: article
date_added: 2026-02-02
source: "https://x.com/i/article/2018370018661027840"
author: "Tom Johnson (tomjohndesign)"
tags: []
via: "Twitter bookmark from @tomjohndesign"
---

Tom Johnson's 9-step design workflow that integrates AI coding tools (Claude Code, conductor_build) into the design process, treating Figma as the last step rather than the first. The process starts from voice dictation and unstructured brain dumps, builds a deliberately bad AI prototype, uses it as a creative director's redlining surface, gutts the codebase and saves only context/constraints as markdown, then moves into Figma for high-craft visual design before rebuilding cleanly from the annotated mockups.

The key reframe: AI is terrible at design (information architecture, affordances, microcopy, layout) but the cost to switch away from poorly made AI decisions is now effectively zero. A garbage scaffold becomes valuable because you can iterate through it 10 times a day to find edge cases, missing states, and the right information hierarchy—before ever touching Figma. The "Step 3: Bad Build" is intentionally terrible and that's the point.

Step 6 (Gut it and save context) is the pivot: instead of continuing to refine messy AI-generated code, the designer asks Claude to write a folder of markdown context files capturing history, constraints, and decisions. Then starts fresh with clean context. Step 8 rebuilds from scratch using Figma mockups + context docs in a new conversation, with the Figma MCP flagged as underpowered—screenshots aren't sufficient, ideally it would pass component names, color tokens, layout structure, and prototype JSON.

## Key Takeaways

- Figma is now step 7, not step 1—most ideation happens before entering the visual design tool
- The "Bad Build" phase has non-zero value: it surfaces missing states, edge cases, and UX gaps you can't see on a blank canvas
- Zero-cost iteration changes the calculus: you can start from scratch 10 times in a day to find emergence
- Markdown context dump (Step 6) before clean rebuild is the most underrated step in the workflow
- The Figma→AI handoff is still the weakest link: MCP is underpowered, screenshots miss component structure and token data
- Final developer handoff still requires a qualified engineer for performance, API integration, and production code decisions

## Links

- [Article](https://x.com/i/article/2018370018661027840)
- [Original Tweet](https://x.com/tomjohndesign/status/2018385296610746403)
