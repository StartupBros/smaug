---
title: "Why your AI agents still don't work"
type: article
date_added: 2026-01-21
source: "https://x.com/i/article/2012902352232058880"
author: "@Abhigyawangoo (abhi)"
tags: []
via: "Twitter bookmark from @Abhigyawangoo"
---

A practitioner's guide to building agents that genuinely improve over time, written by someone who owned agent infra used by millions and now builds self-improving agents for businesses. The core thesis: RAG and retrieval alone aren't enough — the missing ingredient is feedback loops driven by carefully chosen signals that represent real business outcomes. Agents fail because builders optimize for vague metrics (thumbs up/down) instead of multi-dimensional signal sets, which causes reward hacking and reward overoptimization.

The author walks through a full system: start by defining a business metric (retention, conversions, feature activation), then instrument multi-dimensional signals per message (response time delta, conversation abandonment, follow-up clicked, user sentiment), design UI to passively collect those signals (follow-up buttons, link tracking, tab completions), build a signal-derived ranker that scores historical conversations by signal quality and injects the top-10 most similar high-quality examples at generation time, then run controlled A/B experiments to validate every change.

The article includes a ready-to-use Claude Code prompt (Step 5) that walks through implementing the entire feedback loop system into an existing codebase: signal capture hooks, storage schema, UI improvements, embedding-based ranker, A/B framework, and monitoring dashboards.

## Key Takeaways

- Define the business outcome first (retention/conversions/goal achievement) — it determines everything else
- Use 5–10 balanced signals per message; a single signal leads to reward hacking (agent optimizes for negative/sycophantic responses if only response time is measured)
- The highest-lift improvement is few-shot examples ranked by signal quality, not system prompt changes
- Every change needs an experiment against a control group — 50k messages per group for B2C products
- Role shift: agent builders become product designers who write requirements, not engineers who write code

## Links

- [Article](https://x.com/i/article/2012902352232058880)
- [Original Tweet](https://x.com/Abhigyawangoo/status/2013823175855923640)
