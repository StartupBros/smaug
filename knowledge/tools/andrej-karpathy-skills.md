---
title: "andrej-karpathy-skills"
type: tool
date_added: 2026-01-27
source: "https://github.com/forrestchang/andrej-karpathy-skills"
tags: []
via: "Twitter bookmark from @jiayuan_jy"
---

A single `CLAUDE.md` file distilling Andrej Karpathy's publicly-stated observations about LLM coding pitfalls into four actionable principles for Claude Code. Rather than restate generic coding rules, it directly addresses the failure modes Karpathy identified: silent wrong assumptions, overengineered abstractions, orthogonal side-effect edits, and imperative rather than goal-driven task framing. Available both as a Claude Code plugin (installable via the marketplace) and as a per-project `CLAUDE.md` via curl.

## Key Features

- **Think Before Coding**: surface ambiguities and present tradeoffs before starting implementation rather than silently picking an interpretation
- **Simplicity First**: minimum code that solves the problem — no speculative abstractions, no error handling for impossible cases, rewrite if 200 lines could be 50
- **Surgical Changes**: touch only what the request requires; mention but don't delete unrelated dead code; remove only orphans YOUR changes created
- **Goal-Driven Execution**: transform imperative instructions into declarative success criteria with verifiable loops, enabling longer autonomous agent runs

## Links

- [GitHub](https://github.com/forrestchang/andrej-karpathy-skills)
- [Original Tweet](https://x.com/jiayuan_jy/status/2015998216517583211)
