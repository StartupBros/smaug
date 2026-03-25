---
title: "Symphony"
type: tool
date_added: 2026-03-25
source: "https://github.com/openai/symphony"
tags: [ai-agents, workflow-automation, project-management, autonomous-implementation]
via: "Twitter bookmark from @odysseus0z"
---

Symphony turns project work into isolated, autonomous implementation runs, allowing teams to manage work instead of supervising coding agents. It dispatches work from project management systems (like Linear) to autonomous AI agents that implement solutions independently.

## Key Features

- Dispatches work tickets to autonomous implementation agents
- Isolated, autonomous implementation runs per task
- Minimal architecture: cron job + Linear integration
- Uses Linear comments as draft pad for persisted agent state
- Provides proof of work (CI status, PR review feedback, complexity analysis)
- Agents can land PRs safely when tasks are accepted
- Teams manage work at higher level instead of supervising agents

## How It Works

Symphony works as a simple loop:
1. Cron job monitors Linear board for new tickets/tasks
2. Dispatches each ticket to a worker agent
3. Worker maintains state using Linear comment thread as draft pad
4. Agent completes implementation and opens PR
5. Provides detailed proof of work and results
6. When accepted, agents land the PR autonomously

## Architecture Highlights

- **Beautifully designed and minimal** — emphasizes simplicity and elegance
- **Reference Implementation** — Elixir-based example with full setup instructions
- **Specification** — Clear spec for implementing in any programming language
- **Harness Engineering** — Builds on OpenAI's harness engineering approach for better AI integration

## Links

- [GitHub](https://github.com/openai/symphony)
- [Original Tweet](https://x.com/odysseus0z/status/2030413782036726181)
- [OpenAI Harness Engineering](https://openai.com/index/harness-engineering/)
