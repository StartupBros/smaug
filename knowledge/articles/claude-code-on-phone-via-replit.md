---
title: "Run Claude Code on your phone in 5 minutes"
type: article
date_added: 2026-01-19
source: "https://x.com/i/article/2013453084614107136"
author: "matt palmer"
tags: []
via: "Twitter bookmark from @mattyp"
---

A concise step-by-step guide for running Claude Code on a mobile device using Replit as the cloud container. The trick is that Replit hosts the environment on a remote server and supports real-time multiplayer access across devices, so the same Claude Code session started on a laptop becomes accessible via the Replit mobile app's built-in shell. Credentials are persisted in a `.claude-user` directory that survives container restarts. The author provides a pre-configured Replit template to skip manual setup — the whole process from zero to a working mobile Claude Code session takes under five minutes and 500 words of instructions.

## Key Takeaways

- Replit's cloud containers run on remote servers, making any shell session accessible from mobile
- Use the provided Replit template to skip manual Claude Code installation and configuration
- Credentials written to `.claude-user` persist across Replit restarts via the Secrets mechanism
- The mobile Replit shell syncs in real time with the desktop session ("multiplayer")
- Skills, MCP servers, hooks, and plugins all install normally within the Replit environment
- Security note: never make the Replit app public without first deleting the `.claude-user` directory

## Links

- [Article](https://x.com/i/article/2013453084614107136)
- [Original Tweet](https://x.com/mattyp/status/2013466276824523180)
