---
title: "Shell + Skills + Compaction: Tips for long-running agents that do real work"
type: article
date_added: 2026-02-12
source: "https://developers.openai.com/blog/skills-shell-tips/"
author: "OpenAI Developers"
tags: []
via: "Twitter bookmark from @AlexFinn"
---

OpenAI's developer blog post lays out practical patterns for building reliable long-running agent workflows using three primitives in the Responses API: hosted shell, skills, and server-side compaction. The piece is aimed at developers who want agents to run multi-hour workflows without breaking down — addressing the context window exhaustion, state management, and tool coordination problems that plague naive agent implementations.

## Key Takeaways

- Hosted shell gives agents persistent execution environments that survive across API calls, enabling real multi-step work like file editing, test running, and deployment
- Skills let you package reusable capabilities as discrete units the agent can invoke, keeping prompts focused and reducing context bloat
- Server-side compaction handles the context window problem by summarizing earlier conversation history automatically, allowing indefinitely long runs
- Combining all three enables patterns like "plan → execute → verify" loops that can run unattended for hours on real engineering tasks

## Links

- [Article](https://developers.openai.com/blog/skills-shell-tips/)
- [Original Tweet](https://x.com/AlexFinn/status/2021740954244550839)
