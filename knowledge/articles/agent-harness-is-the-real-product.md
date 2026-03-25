# Agent Harness is the Real Product

- **Source:** https://x.com/i/article/2028095934169780224
- **Via:** [@marsBuilds](https://x.com/marsBuilds/status/2028148920895889698)
- **Date:** March 1, 2026

## Summary

The agent harness — execution loop, tool definitions, context management, error recovery — matters more than the underlying model. Evidence: Claude Opus 4.5 scores 42% on CORE-Bench with one scaffold and 78% with another. Cursor's lazy tool loading cuts token usage by 46.9%. Vercel deleted 80% of their agent's tools and watched it go from failing to succeeding.

## Key Architecture Patterns

**The universal loop:**
```
while (model returns tool calls):
    execute tool → capture result → append to context → call model again
```
Every production agent (Claude Code, Cursor, Manus, Devin) runs this loop. The engineering is in what surrounds it.

**Progressive disclosure** — the most underrated pattern: agents discover context incrementally instead of loading everything upfront. Borrowed from UX design (John Carroll, IBM, 1980s; Jakob Nielsen 1990s). Keeps inputs small and places fresh information at the end (high-attention zone), countering the U-shaped LLM attention curve.

## Per-System Notes

**Claude Code:**
- ~18 primitive tools in four categories: discovery (Bash, Glob, Grep, LS), file interaction (Read, Write, Edit, MultiEdit), web (WebSearch, WebFetch), orchestration (TodoWrite, Task)
- Information loaded in six layers at session start: org policies, project CLAUDE.md, user settings, MEMORY.md, session history, git state
- `TodoWrite` does nothing functionally — it's a harness trick forcing the agent to articulate and track its plan
- Skills stored in `.claude/skills/` load on-demand, not every session

**Cursor:**
- Tunes harness per frontier model: different tool names, prompts, behavioral guidance for OpenAI vs Claude
- Files as the fundamental context primitive (searchable, groupable, versionable)
- Semantic search model trained on agent session traces; 12.5% higher accuracy, 2.6% better code retention on large codebases
- Lazy MCP tool loading: gives agent only tool names statically, fetches full definitions on demand → 46.9% token reduction

**Manus:**
- Uses logit masking instead of dynamic tool loading — all ~29 tools stay loaded, availability controlled by constraining output token probabilities during decoding (avoids KV-cache invalidation)
- Hierarchical action space: Level 1 (atomic tool calls), Level 2 (sandbox utilities via Bash), Level 3 (dynamic scripts)
- Biggest gains came from removing things, not adding them

**SWE-Agent:**
- Linter-gated edits: edit rejected if syntactically invalid, agent must retry. Without this, performance drops 3%
- Observation compression: all but last 5 observations collapsed to one line each

**Others:**
- Devin: isolated VMs, Playbook system for repeated tasks, KMS for codified feedback. 67% PR merge rate (up from 34%)
- Windsurf: two-agent architecture — background planning agent + primary action model. "Memories" system for codebase patterns
- Aider: PageRank-based repo map using tree-sitter; binary search to fit critical content in token budget
- Replit: three-agent (Manager, Editor, Verifier) after single-agent error rates were too high

## Quantitative Evidence

| Comparison | Result |
|---|---|
| Claude Opus 4.5, scaffold A vs B | 42% vs 78% on CORE-Bench |
| Cursor lazy tool loading | 46.9% token reduction |
| Vercel: removed 80% of tools | Tokens 145k→67k, steps 100→19, latency 724→141s, failing→succeeding |
| LangChain deepagents-cli harness change | 52.8% → 66.5% on TerminalBench 2.0 (+13.7 pts) |
| Claude-Mem static vs progressive loading | 25,000 tokens at 0.8% efficiency vs 955 tokens at 100% |

## Industry Disagreements

- **Tool overload:** Manus uses logit masking (all tools loaded, constrain outputs) vs Cursor's lazy loading (load on demand). Both work.
- **Context window vs harness filtering:** Google bets on 2M token windows + let the model figure it out. Everyone else actively filters and stages. Harness-heavy approach is winning in practice.

## Key Insight

> "The model is the engine. The harness is the car. Nobody buys an engine."

Dex Horthy (12 Factor Agents): push past 40% of model's input capacity and you enter the "dumb zone" — signal-to-noise degrades and mistakes that look like reasoning failures are actually information overload.

The pattern: best teams keep simplifying. Manus rewrote five times, each time removing things. Claude Code's scaffold is designed to shrink as models improve.

## References

- Anthropic: [Effective Harnesses for Long-Running Agents](https://www.anthropic.com/engineering/effective-harnesses-for-long-running-agents)
- Cursor: [Dynamic Context Discovery](https://cursor.com/blog/dynamic-context-discovery)
- Manus: [Context Engineering for AI Agents](https://manus.im/blog/Context-Engineering-for-AI-Agents-Lessons-from-Building-Manus)
- LangChain: [Improving Deep Agents with Harness Engineering](https://blog.langchain.com/improving-deep-agents-with-harness-engineering/)
- Yang et al.: [SWE-agent (NeurIPS 2024)](https://arxiv.org/abs/2405.15793)
- Liu et al.: [Lost in the Middle (TACL 2024)](https://arxiv.org/abs/2307.03172)
- Horthy: [12 Factor Agents](https://paddo.dev/blog/12-factor-agents/)
