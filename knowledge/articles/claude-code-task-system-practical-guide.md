---
title: "Claude Code's New Task System: The Practical Guide and Explainer"
type: article
date_added: 2026-01-23
source: "https://x.com/i/article/2014647141281464321"
author: "Numman Ali"
tags: []
via: "Twitter bookmark from @nummanali"
---

A deep-dive community explainer covering Claude Code's new dependency-aware Task orchestration system that replaces flat to-do lists. The article walks through all four core tool calls (TaskCreate, TaskUpdate, TaskGet, TaskList), the JSON schema for stored task files, and the mechanics of how blocked/blocking relationships enforce execution order. It covers the full agent delegation model — how Claude assigns tasks to named owners, spawns parallel subagents of different types (general-purpose, Bash, Explore, Plan), and how agents discover and claim their assigned work by polling TaskList.

Critically, the article explains persistence modes: within a session tasks survive context compaction automatically; across sessions you use `CLAUDE_CODE_TASK_LIST_ID` either per-terminal or in `.claude/settings.json`. It includes worked examples from simple (add a logout button) to complex (JWT auth refactor with parallel investigation tasks) to non-code (wedding planning dependency graph).

## Key Takeaways

- Four tool types for agent subtasks: general-purpose (read/write/run), Bash (terminal only), Explore (read-only navigation), Plan (read-only architecture)
- Task dependency chains prevent out-of-order execution; when a blocking task completes, dependent tasks automatically become available
- Tasks stored at `~/.claude/tasks/<list-id>/` as individual JSON files — inspectable, editable, git-trackable externally
- Model selection for subagents: haiku for simple/fast, sonnet for most coding, opus for complex reasoning
- The `activeForm` field ("Running database migrations" not "Doing stuff") improves UI progress display
- Use Tasks for any multi-step work with dependencies, cross-session continuity, or parallel agent delegation; skip for one-shot simple edits

## Links

- [Article](https://x.com/i/article/2014647141281464321)
- [Original Tweet](https://x.com/nummanali/status/2014684862985175205)
