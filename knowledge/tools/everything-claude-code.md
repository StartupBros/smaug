---
title: "everything-claude-code"
type: tool
date_added: 2026-01-21
source: "https://github.com/affaan-m/everything-claude-code"
tags: ["ai-agents", "anthropic", "claude", "claude-code", "developer-tools", "llm", "mcp", "productivity"]
via: "Twitter bookmark from @Gorden_Sun"
---

A production-grade configuration and harness system for Claude Code that won the Anthropic hackathon. Goes beyond config files to provide a complete performance optimization system: skills (domain knowledge packs), agents (specialized subagents for planning, architecture, security review, etc.), hooks (event-triggered automations), commands (slash-command shortcuts), rules (constitutional constraints), and MCP configs (pre-wired integrations with GitHub, Supabase, Vercel, and more). Evolved over 10+ months of intensive daily use building real products.

## Key Features

- Specialized subagents: planner, architect, tdd-guide, security-reviewer, build-error-resolver, e2e-runner, refactor-cleaner
- Skills packs: backend-patterns, frontend-patterns, coding standards, security guidelines
- Slash commands: /tdd, /e2e, /refactor-clean, /test-coverage with automated workflows
- Hooks: auto-format on edit, TypeScript checks, console.log warnings, git push review gates
- MCP configs: GitHub, Supabase, Vercel, Railway, Cloudflare, ClickHouse, Ableton, and more
- Selective install architecture with manifest-driven pipeline (v1.9.0+)
- Available as npm packages: ecc-universal and ecc-agentshield

## Links

- [GitHub](https://github.com/affaan-m/everything-claude-code)
- [Original Tweet](https://x.com/Gorden_Sun/status/2013925532925317459)
