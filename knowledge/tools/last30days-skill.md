---
title: "last30days-skill"
type: tool
date_added: 2026-01-25
source: "https://github.com/mvanhorn/last30days-skill"
tags: ['ai-skill', 'claude-code', 'research', 'reddit', 'twitter', 'hackernews', 'youtube', 'polymarket']
via: "Twitter bookmark from @mvanhorn"
---

A Claude Code skill (installable via `/plugin marketplace add mvanhorn/last30days-skill`) that researches any topic across Reddit, X/Bluesky, YouTube, TikTok, Instagram, Hacker News, Polymarket, and the open web from the past 30 days, then synthesizes a grounded narrative with real citations. The pitch: "The AI world reinvents itself every month. This skill keeps you current." 7,769 stars on GitHub. Written in Python.

Key features include comparative mode (e.g. `/last30 cursor vs windsurf` runs 3 parallel research passes with a side-by-side table and verdict), auto-save to `~/Documents/Last30Days/` for building a personal research library, and per-project `.env` config for API keys. Bluesky/AT Protocol is supported via opt-in credentials. Available on ClawHub as `last30days-official`.

## Key Features

- Multi-platform research: Reddit, X, Bluesky, YouTube, TikTok, Instagram, HN, Polymarket, open web
- Comparative mode: `/last30 X vs Y` produces side-by-side comparison with data-driven verdict
- Auto-saves complete briefings as Markdown files to `~/Documents/Last30Days/`
- 455+ tests across all modules
- Per-project config via `.claude/last30days.env`
- Available on ClawHub: `clawhub install last30days-official`

## Links

- [GitHub](https://github.com/mvanhorn/last30days-skill)
- [Original Tweet](https://x.com/mvanhorn/status/2015551849710190697)
