---
title: "How to 10x your Claude Skills (using Karpathy's autoresearch method)"
type: article
date_added: 2026-03-17
source: "https://x.com/i/article/2033576301383061504"
author: "Ole Lehmann"
tags: []
via: "Twitter bookmark from @itsolelehmann"
---

Ole Lehmann describes a technique for autonomously improving Claude Code skills by adapting Andrej Karpathy's "autoresearch" method — a loop where an AI agent makes one small change to a prompt, scores the output against a yes/no checklist, keeps the change if the score improves and reverts it otherwise, then repeats. The only human input required is defining the checklist (3–6 yes/no quality questions). Lehmann built this as a downloadable Claude Code / Cowork skill: you invoke it on any underperforming skill, set test inputs and checklist questions, and a live browser dashboard tracks scores round-by-round. His landing page copy skill went from 56% to 92% pass rate across four rounds with zero manual edits. The system produces a saved improved skill file, a results log, and a full changelog of every change tried and its outcome — useful for bootstrapping future model upgrades.

## Key Takeaways

- Adapts Karpathy's autoresearch loop to prompt engineering: change one thing, measure, keep or revert
- Scoring uses a tight checklist of 3–6 binary yes/no questions; more than 6 causes the skill to game the checklist
- Live browser dashboard refreshes every 10 seconds with score history and per-question pass/fail breakdown
- Stops autonomously at 95%+ pass rate three consecutive runs; original skill is never overwritten
- Method generalizes beyond skills to anything measurable: page load speed (1100ms → 67ms), cold outreach, newsletter intros

## Links

- [Article](https://x.com/i/article/2033576301383061504)
- [GitHub](https://github.com/olelehmann100kMRR/autoresearch-skill)
- [Original Tweet](https://x.com/itsolelehmann/status/2033919415771713715)
