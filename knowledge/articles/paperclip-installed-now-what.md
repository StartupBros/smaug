---
title: "Installed Paperclip, Now What!?"
type: article
date_added: 2026-03-19
source: "https://x.com/i/article/2034626875926990848"
author: "Nick Spisak"
tags: []
via: "Twitter bookmark from @NickSpisak_"
---

A practical follow-up to a 2.7M-view article on Paperclip, this piece walks through stacking three open-source AI tools into a functioning "AI company": Paperclip (company dashboard/agent manager), gstack by Garry Tan (15-role engineering team with skills like /qa, /ship, /review), and autoresearch by Andrej Karpathy (autonomous overnight R&D loop). The core workflow: Paperclip assigns goals → autoresearch runs 100 experiments overnight → gstack builds the winning approach → gstack ships it. The author frames the human role as "board of directors" — reviewing dashboards, approving sprints, and setting goals rather than writing code.

## Key Takeaways

- Paperclip installs in two minutes via `npx paperclipai onboard --yes`, creates an org chart with budgets and a ticket system
- gstack provides 15 specialist Claude Code skills including `/office-hours` (idea planning), `/plan-ceo-review` (scope challenge), `/qa` (browser-based testing), and `/ship` (full deploy pipeline)
- autoresearch runs iterative experiments autonomously — 5 min/experiment × 12/hr × 8 hrs = ~96 experiments overnight
- The three tools address distinct layers: company management, engineering execution, and R&D experimentation
- Power move: run 10–15 gstack skills simultaneously across different agents and tasks
- `/careful` and `/freeze` modes prevent destructive actions during debugging or production work
- Recommended start: one agent, one goal — hire a CEO, let it suggest first hires, grow organically

## Links

- [Article](https://x.com/i/article/2034626875926990848)
- [Original Tweet](https://x.com/NickSpisak_/status/2034635430700679445)
