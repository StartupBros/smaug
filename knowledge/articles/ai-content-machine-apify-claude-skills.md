---
title: "how I built an AI-powered content machine in 2 hours (6 steps)"
type: article
date_added: 2026-01-22
source: "https://x.com/i/article/2014345180455800832"
author: "Corey Ganim"
tags: []
via: "Twitter bookmark from @coreyganim"
---

Corey Ganim documents a six-step system for building a LinkedIn content engine using Apify for scraping competitor posts, Claude for pattern analysis, and custom Claude Skills for repeatable content generation. The system's distinguishing feature is that it grounds everything in scraped real-world data rather than generic writing prompts, producing templates and hooks that are validated against actual engagement metrics from the creator's niche.

The workflow: compile 10-20 top niche creators, scrape their posts via Apify's LinkedIn Post Search Scraper, have Claude convert and analyze the JSON data for both quantitative patterns (engagement thresholds, media type impact, post length) and qualitative patterns (hook structures, CTA placement, formatting conventions), then encode the discovered formulas into reusable Claude Skills. Key data findings from his run: images outperformed video 70.5% to 8% of top posts, CTAs appeared in 85% of top-decile posts, and longer posts (1,559 chars) outperformed shorter ones (1,268 chars). The process takes about 2 hours and produces three durable reference assets plus two Skills.

## Key Takeaways

- Full data pipeline: Apify scraper → Claude JSON-to-CSV → pattern analysis → Claude Skills
- Two Skills created: `linkedin-hook-writer` (7 proven formulas) and `linkedin-post-writer` (6 tested templates)
- Three reference files: hook swipe file, post templates, pattern playbook with benchmarks
- A separate Brand Voice skill filters all output to maintain individual voice rather than mimicking scraped creators
- Framework is platform-agnostic — designed for LinkedIn but applicable to any content platform

## Links

- [Article](https://x.com/i/article/2014345180455800832)
- [Original Tweet](https://x.com/coreyganim/status/2014357084364509211)
