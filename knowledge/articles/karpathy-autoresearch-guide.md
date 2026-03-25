---
title: "The Ultimate Autoresearch Guide"
type: article
date_added: 2026-03-25
source: "https://www.aibyaakash.com/p/autoresearch-guide"
author: "Aakash Gupta"
tags: [ai-research, autonomous-agents, karpathy, autoresearch, optimization]
via: "Twitter bookmark from @aakashgupta"
---

Aakash Gupta's deep dive into Karpathy's autoresearch project — arguing that most coverage missed the bigger story. The fictional README intro isn't flavor text; it's the spec for what Karpathy is actually building.

The key insight: the 3-file loop (agent edits one file, can't touch another, follows your instruction file) is a general-purpose optimization engine. Score goes up → git commit. Score goes down → git reset. Twelve cycles per hour, a hundred overnight.

## Key Takeaways

- The 3-step roadmap hidden in the README: (1) single-agent loop (shipped), (2) async multi-GPU collaboration like SETI@home, (3) staged self-improvement where small models find improvements that larger models validate and absorb
- Works on anything scoreable: ad copy, cold emails, video scripts, job posts, skill files — not just ML benchmarks
- Tobi Lutke ran it on Shopify's Liquid templating engine: 53% faster rendering from 93 automated commits
- Shopify CEO: 19% gain from 37 overnight experiments on company data
- 42k GitHub stars in a week, 5.8k forks — distributed community GPU surface already exists
- Guide covers six non-ML use cases, the three-step setup, and eval mistakes that kill runs early

## Links

- [Article](https://www.aibyaakash.com/p/autoresearch-guide)
- [Original Tweet](https://x.com/aakashgupta/status/2036666385099870394)
