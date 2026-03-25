---
title: "How to 10x Your Claude Skills (Using Karpathy's Autoresearch Method)"
type: article
date_added: 2026-03-17
source: "https://x.com/i/article/2033576301383061504"
author: "Ole Lehmann"
tags: [claude-code, skills, autoresearch, karpathy, prompt-optimization, agents]
via: "Twitter bookmark from @itsolelehmann"
---

Ole Lehmann adapts Karpathy's autoresearch loop to auto-improve Claude Code skills. The core idea: define a yes/no scoring checklist (3–6 questions), kick off the agent, and it iterates — making one small change per round, keeping it if the pass rate rises, reverting if it drops — until hitting 95%+ three times in a row.

His landing page copy skill went from 56% to 92% pass rate in four rounds with zero manual intervention. Changes included adding a banned buzzword list, requiring a specific number in the headline, and inserting a worked example. One change (tighter word count) was auto-reverted because it degraded the CTA quality.

## Key Takeaways

- Scoring checklist should be yes/no binary questions (not numeric ratings) for consistent evaluation across runs
- 3–6 questions is the sweet spot — more causes the skill to "game the checklist" like a student memorizing answers
- A live dashboard auto-refreshes every 10 seconds showing score chart, per-question pass/fail breakdown, and a change log
- The skill saves the improved version separately, leaving the original untouched
- The method works on anything scoreable: page load times, cold outreach emails, newsletter intros, any repeatable prompt
- The change log itself is valuable — a record of what works/doesn't that transfers to future, smarter models

## Links

- [Article](https://x.com/i/article/2033576301383061504)
- [GitHub](https://github.com/olelehmann100kMRR/autoresearch-skill)
- [Original Tweet](https://x.com/itsolelehmann/status/2033919415771713715)
