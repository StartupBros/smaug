---
title: "We turned Openclaw into a self improving vibe marketer for our $300,000/yr app."
type: article
date_added: 2026-03-17
source: "https://x.com/i/article/2032650605236203521"
author: "Ernesto Lopez"
tags: []
via: "Twitter bookmark from @ErnestoSOFTWARE"
---

Ernesto Lopez describes a fully autonomous ad creation pipeline built on top of the Openclaw agent "Eddie." The system uses Apify to scrape the Meta Ad Library for competitor video ads, runs each through OpenAI Whisper for transcription, extracts winning hooks and angles, then rewrites them in the brand's voice using a set of markdown files (writing-rules.md, voice.md, product.md, icp.md). Scripts are distributed to either UGC creators ($15–50/video) or pushed via API to Arcads for AI actor renders — producing 50+ finished ads in minutes. Post-run CPA data flows back through Singular's MMP API so Eddie can double down on winning creative directions. The result is a generate → evaluate → regenerate loop that runs mostly without human involvement and is actively scaling a $300k/yr app toward $1M/yr.

## Key Takeaways

- Competitor ad intelligence is automated end-to-end: Apify scrapes Meta Ad Library, Whisper transcribes, Eddie analyzes and rewrites
- Brand voice is encoded in markdown files that act as an "anti-AI filter" trained on the Wikipedia article on signs of AI writing
- Two-track distribution: top scripts go to human UGC creators; remainder are bulk-rendered by Arcads AI actors
- Performance data closes the loop via MMP API — the system improves on every cycle without manual intervention
- 100+ creatives tested per month with Meta deciding which to push

## Links

- [Article](https://x.com/i/article/2032650605236203521)
- [Original Tweet](https://x.com/ErnestoSOFTWARE/status/2033917717762191659)
