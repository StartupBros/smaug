---
title: "You Could've Invented OpenClaw"
type: article
date_added: 2026-02-11
source: "https://x.com/i/article/2021347850656022528"
author: "nader dabit"
tags: []
via: "Twitter bookmark from @dabit3"
---

Dabit reverse-engineers OpenClaw by building it from scratch in a tutorial, starting with the simplest possible Telegram bot and incrementally adding each capability that makes OpenClaw what it is. The article is both a conceptual explainer and working code guide — each step adds one piece of the architecture and explains the design decision behind it.

The four core problems with browser-based AI (stateless, passive, isolated, single-channel) map to four architectural solutions OpenClaw implements: persistent filesystem memory, scheduled task runners, tool use with shell/browser access, and a channel gateway that normalizes messages from Telegram, Discord, WhatsApp, Slack, and iMessage into a single agent context. The article covers session scoping strategies, semantic browser snapshots via Playwright accessibility trees (100x cheaper than screenshots), vector memory with hybrid FTS5/embedding search, and sub-agent spawning via `sessions_spawn`.

## Key Takeaways

- Persistent memory is just files: conversations, preferences, and project state live on disk, giving the agent durable context across restarts
- Playwright semantic snapshots replace screenshots with accessibility-tree text, cutting token cost ~100x and making browser interactions ref-based rather than positional
- Session scoping options (main / per-peer / per-channel-peer) plus identity links enable flexible memory isolation between users and channels
- Channel plugin architecture normalizes all messaging surfaces into one common format — adding a new channel only requires a single adapter
- Sub-agent spawning lets a parent agent delegate long-running tasks and resume when results return
- The step-by-step build makes the OpenClaw architecture fully legible: messaging API + LLM + filesystem = persistent AI assistant

## Links

- [Article](https://x.com/i/article/2021347850656022528)
- [Original Tweet](https://x.com/dabit3/status/2021387483364151451)
- [Code Gist](https://gist.github.com/dabit3/bc60d3bea0b02927995cd9bf53c3db32)
