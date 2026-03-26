---
title: "aeon"
type: tool
date_added: 2026-03-23
source: "https://github.com/aaronjmars/aeon"
tags: []
via: "Twitter bookmark from @aaronjmars"
---

Aeon is a Claude Code skill system for scheduling and automating agentic tasks within a Claude Pro/Max subscription window. It monitors the 5-hour rate-limit window via Anthropic's `/api/oauth/usage` endpoint and triggers queued skills (PR fixes, research tasks, etc.) when less than 30 minutes remain in the window — ensuring the subscription is fully utilized before the reset.

## Key Features

- Monitors Claude's 5-hour rate-limit window via the official API endpoint
- Triggers scheduled skills automatically before window expiration
- Designed to maximize utilization of Claude Pro/Max subscription limits
- Author uses it for PR fixes and research tasks as background scheduled work

## Links

- [GitHub](https://github.com/aaronjmars/aeon)
- [Original Tweet](https://x.com/aaronjmars/status/2036230574822580675)
