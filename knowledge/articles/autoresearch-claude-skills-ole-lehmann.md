---
title: "How to 10x Your Claude Skills Using Karpathy's Autoresearch Method"
type: article
date_added: 2026-03-24
source: "https://x.com/i/article/2033576301383061504"
author: "Ole Lehmann"
tags: [claude, skills, autoresearch, karpathy, prompt-optimization, cowork, autonomous-agents]
via: "Twitter bookmark from @shannholmberg"
---

Ole Lehmann's guide to applying Andrej Karpathy's autoresearch loop to auto-improve Claude skill prompts. You define a 3–6 item yes/no quality checklist, run the agent, and it iteratively mutates the skill prompt — keeping changes that improve the score, reverting ones that don't — until it hits 95%+ pass rate or you stop it. A landing page copy skill improved from 56% to 92% pass rate with zero manual intervention.

## Key Takeaways

- The core loop: run skill → score against checklist → mutate prompt → test again → keep or revert → repeat. Same as ML hyperparameter search but applied to prompt engineering.
- Quality checklist should be yes/no questions (3–6 items), not vague 1–10 ratings. Example for landing page: "Does the headline include a specific number?" / "Is it free of buzzwords?" / "Is the CTA a specific verb phrase?"
- A live dashboard auto-refreshes every 10 seconds with a score chart, pass/fail per checklist item, and a change log. The agent runs fully autonomously until 95%+ three times in a row.
- The method applies to anything scoreable: page load speed, cold outreach copy, newsletter intros, any repeatable prompt.
- The changelog produced at the end is particularly valuable — a record of what works and what doesn't that future models can pick up from.
- Download the autoresearch skill and drop it into Claude Code or Cowork skills folder; also on GitHub at github.com/olelehmann100kMRR/autoresearch-skill.

## Links

- [Article](https://x.com/i/article/2033576301383061504)
- [Original Tweet](https://x.com/shannholmberg/status/2036461256006357409)
- [GitHub](https://github.com/olelehmann100kMRR/autoresearch-skill)
