# The Shorthand Guide to Everything Claude Code

- **Source:** https://x.com/i/article/2012310917812502528
- **Author:** @affaanmustafa (cogsec)
- **Date:** January 16, 2026

## Summary

A comprehensive guide to Claude Code based on 10 months of daily use. Covers the full configuration surface: skills, hooks, subagents, MCPs, plugins, and parallel workflows.

## Skills and Commands

- **Skills** (`~/.claude/skills/`) — broader workflow definitions, rules-like
- **Commands** (`~/.claude/commands/`) — quick executable slash commands
- Skills can include codemaps to help Claude navigate codebases without burning context

## Hooks

Trigger-based automations on tool calls and lifecycle events:

1. `PreToolUse` — before a tool executes (validation, reminders)
2. `PostToolUse` — after a tool finishes (formatting, feedback loops)
3. `UserPromptSubmit` — when user sends a message
4. `Stop` — when Claude finishes responding
5. `PreCompact` — before context compaction
6. `Notification` — permission requests

Use the `hookify` plugin to create hooks conversationally instead of writing JSON manually.

## Subagents

Processes the orchestrator can delegate tasks to with limited scopes. Can run in background/foreground. Configure allowed tools and MCPs per subagent.

Example structure: `~/.claude/agents/` with planner, architect, tdd-guide, code-reviewer, security-reviewer, build-error-resolver, e2e-runner, refactor-cleaner.

## MCPs — Context Window Management

**Critical:** Be selective. 200k context window before compacting may only be 70k with too many tools enabled.

Rule of thumb: Have 20–30 MCPs in config, keep under 10 enabled, under 80 tools active.

## Plugins

Package tools (skill + MCP combined, or hooks/tools bundled). LSP plugins useful for running Claude Code outside editors — gives real-time type checking without an IDE.

Recommended: `typescript-lsp`, `pyright-lsp`, `hookify`, `mgrep`

## Key Tips

- `Ctrl+U` — delete entire line
- `!` — quick bash prefix, `@` — file search, `/` — slash commands
- `Shift+Enter` — multi-line input, `Tab` — toggle thinking, `Esc Esc` — interrupt
- `/fork` — fork conversations for parallel non-overlapping tasks
- Git worktrees for parallel Claude instances without conflicts
- `mgrep` (via plugin) significantly better than ripgrep for both local and web search
- `/rewind`, `/checkpoints`, `/compact`, `/statusline`

## Editor Recommendation

Zed (Rust-based) — lightweight, fast, real-time file change tracking via Agent Panel, `Ctrl+G` to open file Claude is working on.

## Author's Config

**MCPs configured (user level):** github, firecrawl, supabase, memory, sequential-thinking, vercel, railway, cloudflare-docs/workers/observability, clickhouse, AbletonMCP, magic. Only 5–6 enabled per project.

**Key hooks:** tmux reminder for long-running commands, block unnecessary .md creation, prettier/tsc on edit, console.log warnings.

**Rules:** `~/.claude/rules/` with security, coding-style, testing, git-workflow, agents, patterns, performance, hooks.
