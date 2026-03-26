---
title: "Your Claude setup rots over time. Detox it in 60 seconds (with this self-audit prompt):"
type: article
date_added: 2026-03-25
source: "https://x.com/i/article/2036433375150354432"
author: "Ole Lehmann"
tags: [claude-code, claude-md, prompting, workflow, claude-cowork, maintenance]
via: "Twitter bookmark from @itsolelehmann"
---

Ole Lehmann argues that Claude setups accumulate contradictory instructions over time — each rule added to fix a specific bad output, but never removed. The result is over-prompting: the model tries to satisfy 89 conflicting rules simultaneously on every output, degrading quality. Anthropic's own engineering team apparently hit the same problem internally. The fix is a self-audit prompt that tells Claude to read its own setup and flag everything redundant, contradictory, too vague, or added as a bandaid for a one-off problem.

The article provides a full copy-paste self-audit prompt that works especially well with Claude Cowork (desktop app), where Claude already has filesystem access to CLAUDE.md, skills, and context files without the user pasting anything. The five audit filters are: (1) does Claude already do this by default, (2) does it contradict another rule, (3) does it repeat something already covered, (4) was it a bandaid for one bad output, (5) is it too vague to apply consistently. The output is a cut list with reasons, a conflict map between files, and a cleaned-up CLAUDE.md.

The article also describes automating the audit as a weekly scheduled task in Cowork (set it up once, runs every Monday at 9am silently in the background). The broader principle is "addition by subtraction" — a leaner setup consistently outperforms a bloated one, and model updates regularly make old instructions redundant.

## Key Takeaways

- Over-prompting is a real failure mode: accumulated rules from fixing individual bad outputs eventually contradict each other and degrade average output quality
- The self-audit prompt has Claude read its own setup files and apply five filters to flag dead weight — no manual review required
- Running the full audit at once (deleting all flagged rules simultaneously) lets you feel the quality difference clearly, then add back only what actually degrades
- Claude Cowork's scheduling feature can automate the audit weekly, keeping prompt hygiene clean without relying on willpower
- The minimum viable setup — fewest instructions for consistent quality — is the target, not comprehensiveness

## Links

- [Article](https://x.com/i/article/2036433375150354432)
- [Original Tweet](https://x.com/itsolelehmann/status/2036533756572639611)
