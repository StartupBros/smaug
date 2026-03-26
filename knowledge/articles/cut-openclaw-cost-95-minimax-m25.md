---
title: "I cut my OpenClaw cost by 95%"
type: article
date_added: 2026-02-13
source: "https://x.com/i/article/2022272369113649152"
author: "Akshay Pachaar"
tags: []
via: "Twitter bookmark from @akshay_pachaar"
---

Akshay Pachaar switched his entire OpenClaw agent setup from Claude Opus 4.6 to Minimax M2.5, achieving a 95% cost reduction. M2.5 is a Mixture-of-Experts model that activates only 10 billion parameters, scoring 80.2% on SWE-Bench Verified (on par with Opus 4.6 for coding) and 76.8% on BFCL for agentic tool-calling. At roughly $1/hour with 100 tokens per second, it makes long-running autonomous agents economically viable at scale. The article provides a step-by-step setup guide for OpenClaw with Minimax M2.5 via Telegram bots, and describes the author's three-agent setup (Neo the AI engineer, Pulse the daily research briefer, and Pixel the graphic designer) all running 24/7 through Telegram.

## Key Takeaways

- Minimax M2.5 matches Opus 4.6 on coding benchmarks (80.2% SWE-Bench Verified) at ~95% lower cost
- Only 10B active parameters makes it the smallest Tier-1 model — big self-hosting advantage
- Designed for long-horizon agentic tasks; handles complex multi-step workflows without losing context
- Starter Coding Plan on Minimax platform is $8.8/month for production-grade agentic coding
- Practical multi-agent setup via Telegram: one bot per role (engineer, researcher, designer)
- YouTube masterclass linked for full OpenClaw setup walkthrough: https://youtu.be/aFQJYaornJ4

## Links

- [Article](https://x.com/i/article/2022272369113649152)
- [Original Tweet](https://x.com/akshay_pachaar/status/2022309334483677654)
