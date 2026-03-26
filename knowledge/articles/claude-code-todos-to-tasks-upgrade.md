---
title: "We're turning Todos into Tasks in Claude Code"
type: article
date_added: 2026-01-22
source: "https://x.com/i/article/2014473994695823360"
author: "Anthropic"
tags: []
via: "Twitter bookmark from @trq212"
---

Anthropic announced the upgrade of Claude Code's TodoWrite system to a new "Tasks" primitive designed for longer, more complex projects. The core motivation was that as Opus 4.5 became capable of running autonomously for extended periods, flat to-do lists were no longer sufficient — Claude already knew what to do for small tasks and didn't need them, but longer multi-session or multi-agent projects needed better coordination. Tasks are stored as files in `~/.claude/tasks` so multiple subagents and sessions can read and update shared state, with changes broadcast across all active sessions.

The new system supports dependency relationships between tasks (blocking/blocked-by), persistence across sessions via the `CLAUDE_CODE_TASK_LIST_ID` environment variable, and agent delegation patterns. This is partly inspired by Steve Yegge's "Beads" project.

## Key Takeaways

- Tasks replace the TodoWrite tool for complex, multi-step work spanning multiple sessions or subagents
- Tasks are stored in the filesystem (`~/.claude/tasks`) enabling real collaboration across context windows
- Set `CLAUDE_CODE_TASK_LIST_ID=<name> claude` to persist a task list across separate sessions
- Dependency management ensures Claude won't start work that requires unfinished prerequisites
- Multiple parallel subagents can all read from and write to the same task list without conflicts

## Links

- [Article](https://x.com/i/article/2014473994695823360)
- [Original Tweet](https://x.com/trq212/status/2014480496013803643)
