---
title: "How my OpenClaw agent, Larry, got millions of TikTok views in one week. (Full step-by-step guide)"
type: article
date_added: 2026-02-12
source: "https://x.com/i/article/2021875898064990208"
author: "Oliver Henry"
tags: []
via: "Twitter bookmark from @oliverhenry"
---

Oliver Henry's detailed walkthrough of building Larry — an OpenClaw AI agent running on an old gaming PC — that fully automates TikTok slideshow creation and posting for two iOS apps (Snugly and Liply). Within five days the system generated 500K+ views and pushed MRR to $588, with individual posts hitting 234K, 167K, and 147K views. The article is co-written with Larry itself and covers every component: image generation via gpt-image-1.5, text overlay code, posting through the Postiz API as TikTok drafts, and the skill/memory file system that makes the agent compound in capability over time.

The core breakthrough was hook formula: "[Another person] + [conflict or doubt] → showed them AI → they changed their mind." Self-focused hooks (features, price comparisons) consistently failed. Hooks framing a human moment with another character — landlord, mum, boyfriend — routinely cleared 100K views. The architecture lock trick for consistent rooms across 6 slides (freeze all structural elements, vary only style) solved the continuity problem that killed early attempts with Stable Diffusion.

## Key Takeaways

- OpenClaw + local Linux machine + gpt-image-1.5 + Postiz API = fully autonomous TikTok content pipeline for ~$0.50/post ($0.25 with Batch API)
- Skill files (markdown documents encoding workflows, rules, and failure logs) are the compounding advantage — they make the agent smarter after every failure
- Portrait orientation (1024x1536), exactly 6 slides, and locked room architecture across slides are non-negotiable technical requirements for engagement
- Viral hook formula: frame a human conflict with a third party, not the product's features — "I showed my landlord what AI thinks it could look like" vs. "See your room in 12+ styles"
- Workflow splits 95/5: agent handles generation and drafts, human spends 60 seconds adding trending audio and publishing
- OpenAI Batch API cuts image generation cost in half for pre-scheduled overnight runs

## Links

- [Article](https://x.com/i/article/2021875898064990208)
- [Original Tweet](https://x.com/oliverhenry/status/2022011925903667547)
