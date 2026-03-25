---
title: "Autoresearch Guide: Karpathy's Locked Eval as the Template for AI-Augmented Orgs"
type: article
date_added: 2026-03-23
source: "https://www.aibyaakash.com/p/autoresearch-guide"
author: "Aakash Gupta"
tags: [ai-agents, autoresearch, karpathy, org-design, evaluation, autonomous-agents]
via: "Twitter bookmark from @aakashgupta"
---

Aakash Gupta's analysis of Karpathy's autoresearch three-file architecture as the design pattern for every AI-augmented organization. The key insight: the separation between execution (what the agent edits), evaluation (what is locked and immutable), and strategy (what the human writes) is what makes AI agent results trustworthy.

The locked eval file (val_bpb in Karpathy's case) is the critical innovation. The agent cannot redefine it, cannot swap datasets, cannot adjust tokenizers to make numbers look better. Results held across 700 experiments (20 kept) and transferred to a model twice the size. Shopify's CEO replicated the pattern overnight: 37 experiments, 19% quality improvement.

The Substack article covers six practical use cases, three-step setup, and common eval mistakes.

## Key Takeaways

- Three-file architecture: editable code (agent owns), locked eval (no one touches mid-run), strategy/instructions (human writes)
- "Whoever controls the eval controls the outcome" — locking the eval is what prevents agents from gaming the metric
- Pattern transfers beyond ML: sales (agent writes sequences, locked system scores reply quality), product (agent ships variants, locked analytics measures retention), recruiting (agent screens, calibrated rubric scores)
- 700 experiments → 20 kept → all 20 transferred to 2x larger model = results were real because eval was trustworthy
- The problem in most companies: the person who sets the goal also controls how success is measured — this incentive structure breaks with autonomous agents
- Shopify's Tobi Lutke replicated the pattern: 37 experiments, 19% quality improvement, smaller model beat larger one
- Guide at aibyaakash.com covers: six use cases, three-step setup, eval mistakes that kill runs

## Links

- [Article](https://www.aibyaakash.com/p/autoresearch-guide)
- [Original Tweet](https://x.com/aakashgupta/status/2036006034729304175)
- [Quoted Tweet](https://x.com/aakashgupta/status/2034851259442749909)
