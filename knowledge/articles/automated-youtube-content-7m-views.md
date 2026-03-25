---
title: "We got 7M views on YouTube with completely automated content"
type: article
date_added: 2026-03-08
source: "https://x.com/i/article/2029564042390503424"
author: "Mau Baron (@maubaron)"
tags: [automation, youtube, content, python, claude-code, viral]
via: "Twitter bookmark from @mdnlabs"
---

A walkthrough of a fully automated YouTube Shorts system that reached 7M views and 61k subscribers without manually uploading a single video. The workflow takes ~10 minutes to produce 700 posts by scraping viral video hooks and stitching a CTA clip onto them.

## Key Takeaways
- **Hook strategy**: Use viral creator clips (e.g. ZackD Films) as the first 3 seconds — these act as brainrot hooks that earn attention before transitioning to a CTA.
- **CTA clip**: Create a short branded clip using CapCut with Pinterest images, transitions, and a recognizable viral song.
- **Python scraper**: Claude Code generates a headless browser scraper to download 10 YouTube Shorts from a given creator profile URL.
- **Stitching**: A second Claude Code-generated script grabs the first 3 seconds of each scraped video and appends `CTAvideo.mp4`.
- **Scheduling**: Use any scheduling tool (e.g. Post Bridge by @jackfriks). Manual posting recommended for the first week on YouTube to avoid shadow bans.
- **Warning**: Automated uploading to YouTube risks shadow bans — authors experienced this multiple times.

## Links
- [Article](https://x.com/i/article/2029564042390503424)
- [Original Tweet](https://x.com/mdnlabs/status/2030807267755294988)
