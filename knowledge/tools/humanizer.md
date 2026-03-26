---
title: "humanizer"
type: tool
date_added: 2026-01-18
source: "https://github.com/blader/humanizer"
tags: []
via: "Twitter bookmark from @blader"
---

A Claude Code skill that strips AI writing patterns from text to make it sound more natural and human. Built by Siqi Chen after he noticed Wikipedia had comprehensively catalogued "Signs of AI Writing" — he simply fed that article to Claude Code and asked it to generate a skill that avoids all 25 identified patterns. The skill performs an initial rewrite pass followed by an "obviously AI generated" audit pass and a second rewrite, targeting patterns like significance inflation, AI vocabulary ("testament", "landscape", "showcasing"), em dash overuse, boldface overuse, sycophantic phrases, and formulaic challenges.

## Key Features

- Addresses 25 documented AI writing patterns across content, language, style, communication, and filler categories
- Two-pass approach: initial rewrite + audit pass to catch lingering AI-isms
- Based on Wikipedia's WikiProject AI Cleanup guide, derived from analysis of thousands of AI-generated texts
- Install by cloning directly into `~/.claude/skills/humanizer`
- Invoke with `/humanizer` or by asking Claude to "humanize" text

## Links

- [GitHub](https://github.com/blader/humanizer)
- [Original Tweet](https://x.com/blader/status/2013015738622284156)
