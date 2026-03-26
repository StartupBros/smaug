---
title: "Lessons from Building Claude Code: Seeing like an Agent"
type: article
date_added: 2026-02-27
source: "https://x.com/i/article/2027446899310313472"
author: "Thariq"
tags: []
via: "Twitter bookmark from @trq212"
---

A deep technical essay from the Claude Code team on how to design tool spaces for LLM agents. The core insight is that effective agent tool design requires "seeing like an agent" — understanding the model's capabilities, then shaping tools to match them rather than the other way around. The author walks through three real design problems encountered while building Claude Code: the AskUserQuestion elicitation tool (tried three approaches before landing on a modal-blocking structured form), the evolution from TodoWrite to Task tool as models improved, and the shift from RAG vector search to agent-directed grep search as Claude became capable of building its own context.

## Key Takeaways

- Tools must be shaped to the model's actual abilities — give it primitives that amplify what it's already good at, not generic wrappers
- AskUserQuestion went through three iterations (ExitPlanTool parameter → modified markdown format → dedicated blocking tool) before working well; the tool only works if Claude "wants" to call it
- As model capability increases, previously necessary scaffolding like periodic Todo reminders can become actively constraining — constantly revisit assumptions
- Progressive disclosure (letting Claude incrementally discover context via linked files) lets you add functionality without adding tools to the action space
- The Guide subagent pattern (a specialized subagent for a narrow task) is an underused alternative to stuffing context into the system prompt
- Supporting a small, stable set of models with similar capability profiles makes it easier to reason about tool design decisions

## Links

- [Article](https://x.com/i/article/2027446899310313472)
- [Original Tweet](https://x.com/trq212/status/2027463795355095314)
