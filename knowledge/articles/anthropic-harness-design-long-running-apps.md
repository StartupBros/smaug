---
title: "Harness Design for Long-Running Claude Apps"
type: article
date_added: 2026-03-25
source: "https://www.anthropic.com/engineering/harness-design-long-running-apps"
author: "Prithvi Rajasekaran / Anthropic"
tags: [ai-agents, claude, multi-agent, harness, anthropic]
via: "Twitter bookmark from @iamsupersocks"
---

Summary based on the tweet thread: Anthropic's engineering blog post describing how multi-agent harnesses unlock Claude for long-running tasks. Key problems: context drift and inability to self-evaluate. Solution: separate producer and evaluator agents (inspired by GANs). For frontend: evaluator uses Playwright to navigate and score on 4 criteria, generator iterates 5-15 times. For full apps: 3-agent system (planner, developer, tester). Results: 6 hours autonomous work → complete game editor with sprites, levels, and AI content generation. With Opus 4.6, architecture simplifies while opening new multi-agent combinations.

## Key Takeaways

- Never let an agent evaluate its own work — use a separate evaluator agent
- Producer/evaluator separation is inspired by GANs (generative adversarial networks)
- Frontend loop: Playwright-based evaluator scores visual quality, originality, technical rigor, functionality
- App development loop: planner → developer → tester (user simulation) → developer
- Better models don't make orchestration obsolete — they shift the cursor, enabling new combinations

## Links

- [Article](https://www.anthropic.com/engineering/harness-design-long-running-apps)
- [Original Tweet](https://x.com/iamsupersocks/status/2036504448621511070)
