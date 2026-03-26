---
title: "The Shorthand Guide to Everything Claude Code"
type: article
date_added: 2026-01-21
source: "https://x.com/i/article/2012310917812502528"
author: "@affaanmustafa (cogsec)"
tags: []
via: "Twitter bookmark from @affaanmustafa"
---

A comprehensive reference guide to Claude Code's full feature surface, written by the Anthropic hackathon winner behind the everything-claude-code repo. Covers the author's complete personal setup after 10 months of daily use: skills, hooks, subagents, MCPs, plugins, and productivity tricks. The guide frames configuration as fine-tuning rather than architecture — the goal is a lean, well-scoped system, not a maximalist one.

Skills are workflow definitions scoped to specific tasks (not just markdown files — they can include scripts and tools). Hooks are event-triggered automations firing on PreToolUse, PostToolUse, UserPromptSubmit, Stop, PreCompact, and Notification events. Subagents are delegated processes with limited tool permissions; the author keeps dedicated agents for planning, architecture, TDD, code review, security scanning, and e2e testing. MCPs connect Claude to external services; the critical insight is context window management — have 20–30 MCPs configured but keep under 10 enabled, under 80 tools active. Plugins bundle tools + MCPs + hooks for easy installation.

The author's editor of choice is Zed (Rust-based, instant startup, Agent Panel for real-time file tracking). Key workflow tip: use git worktrees for parallel Claude instances without conflicts, and tmux for long-running commands.

## Key Takeaways

- Context window is precious: too many MCPs/plugins can shrink effective context from 200k to 70k
- Skills should provide tools via scripts, not just markdown context
- Use the `hookify` plugin to create hooks conversationally rather than hand-writing JSON
- /fork forks conversations for non-overlapping parallel tasks; git worktrees for overlapping parallel instances
- Recommended plugins: typescript-lsp, pyright-lsp, hookify, mgrep (better than ripgrep), context7
- Key shortcuts: Ctrl+U (delete line), Tab (toggle thinking), Esc Esc (interrupt/restore)

## Links

- [Article](https://x.com/i/article/2012310917812502528)
- [Original Tweet](https://x.com/affaanmustafa/status/2012378465664745795)
- [everything-claude-code repo](https://github.com/affaan-m/everything-claude-code)
