---
title: "Your Claude Setup Rots Over Time. Detox It in 60 Seconds."
type: article
date_added: 2026-03-24
source: "https://x.com/i/article/2036433375150354432"
author: "Ole Lehmann"
tags: []
via: "Twitter bookmark from @itsolelehmann"
---

Most Claude setups degrade quietly: rules accumulate to fix one-off bad outputs, contradictions pile up, and the model wastes capacity trying to satisfy irrelevant constraints. Deleting half the setup often makes outputs measurably better. The article gives a single self-audit prompt you paste into Claude Cowork — it reads your entire setup (CLAUDE.md, skills folder, context files) without you pasting anything, then evaluates every rule against five filters: default behavior, contradictions, redundancy, bandaid fixes, and vagueness. It returns a cut list with reasons plus a cleaned-up CLAUDE.md.

The core concept is minimum viable setup: the fewest instructions that consistently produce the quality you want. To prevent re-bloat, the article walks through scheduling a weekly audit task in Cowork that runs automatically every Monday morning and reports what to cut — no willpower required.

## Key Takeaways

- Accumulating rules over time degrades model performance; addition by subtraction is real
- Self-audit prompt: tell Claude to read its own setup and score every rule against 5 filters (default behavior, contradictions, redundancy, bandaid, vagueness)
- After getting audit results: delete everything flagged at once, test 3 common tasks, only restore rules where something got worse
- Schedule a recurring weekly audit in Cowork so hygiene runs on autopilot
- Every model update makes some old instructions unnecessary — treat the setup as living documentation that should shrink, not grow

## Links

- [Article](https://x.com/i/article/2036433375150354432)
- [Original Tweet](https://x.com/itsolelehmann/status/2036533756572639611)
