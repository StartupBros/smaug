---
title: "claude-code-showcase"
type: tool
date_added: 2026-01-14
source: "https://github.com/ChrisWiles/claude-code-showcase"
tags: []
via: "Twitter bookmark from @brian_lovin"
---

A comprehensive reference implementation of Claude Code project configuration, showing how to build a production-quality AI-assisted development workflow. Covers the full stack: hooks for automated quality gates (auto-format, type-check, block edits on main), reusable skills for domain knowledge (component libraries, testing patterns, GraphQL schema), specialized subagents for code review and task delegation, slash commands for common workflows, and GitHub Actions for scheduled maintenance (monthly docs sync, weekly code quality scans, biweekly dependency audits). The README includes a skill evaluation hook system that analyzes each prompt and auto-suggests which skills Claude should activate based on keywords and intent patterns.

Brian Lovin shared a prompt template for using this repo to evaluate your own Claude Code setup: point Claude Code at this repo, have it explore the configuration patterns, then systematically compare them against your own `.claude` directory and propose improvements with a before/after testing framework for each suggestion.

## Key Features

- Hooks for auto-formatting, TypeScript type-checking, blocking edits on main, and auditing for `console.log`s
- Skill evaluation system that suggests relevant skills based on prompt keywords and file paths
- JIRA/Linear integration via MCP servers — Claude reads ticket, implements feature, updates status, links PR
- GitHub Actions for scheduled maintenance: docs sync, code quality review, dependency audit
- Code review agent run after every change, plus PR review GitHub Action
- Ticket triage automation: Claude reads the ticket and leaves an implementation comment before an engineer picks it up

## Links

- [GitHub](https://github.com/ChrisWiles/claude-code-showcase)
- [Original Tweet](https://x.com/brian_lovin/status/2011579369710657641)
