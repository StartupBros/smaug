---
title: "Sec-Context: AI Code Security Anti-Patterns"
type: article
date_added: 2026-01-20
source: "https://arcanum-sec.github.io/sec-context/"
author: "Jason Haddix (Jhaddix)"
tags: []
via: "Twitter bookmark from @mrgretzky"
---

A curated collection of security guardrails and anti-patterns distilled from 150+ sources, designed to be included in AI code-gen contexts to prevent LLMs from hallucinating insecure code. Created by Jason Haddix, the library covers the most common vulnerability classes that LLMs introduce when generating code — including injection flaws, insecure defaults, and dependency confusion attacks. The term "slopsquatting" (hallucinated package names threat actors can register) is highlighted as an emerging risk. The files are plain Markdown, so they can be dropped directly into system prompts, CLAUDE.md, or Cursor rules.

## Key Takeaways

- LLMs reliably hallucinate the same vulnerability classes — this project enumerates and documents them
- Security guardrails can be embedded in codegen context as Markdown files, shifting left without changing developer workflow
- "Slopsquatting" — AI hallucinating plausible-but-nonexistent package names — is an actively exploitable supply chain vector
- Reading through the guardrail files is itself a useful webapp security education, beyond just the LLM use case
- Vibe coding without human review of security-sensitive paths creates real production risk, not just tech debt

## Links

- [Article](https://arcanum-sec.github.io/sec-context/)
- [Original Tweet](https://x.com/mrgretzky/status/2013668023459078418)
