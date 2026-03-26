---
title: "Skill Graphs > SKILL.md"
type: article
date_added: 2026-02-18
source: "https://x.com/i/article/2023918991673061376"
author: "Heinrich (arscontexta)"
tags: []
via: "Twitter bookmark from @arscontexta"
---

Heinrich argues that single SKILL.md files hit a ceiling — real agentic depth requires a network of interconnected skill files (a "skill graph") linked via wikilinks. Each node is one complete technique or methodology claim; YAML frontmatter lets the agent scan without reading full files; and wikilinks embedded in prose carry semantic meaning so the agent follows relevant paths without loading everything. The result is progressive disclosure: index → descriptions → links → sections → full content, with most routing decisions made before reading a single full file.

The author's own `arscontexta` plugin is a 249-file skill graph that teaches an agent how to build knowledge bases. Use cases span trading systems (risk management, market psychology, position sizing linked together), legal knowledge (contract patterns, jurisdiction specifics, precedent chains), and company onboarding graphs. The primitives are simple: wikilinks as prose, YAML frontmatter descriptions, and MOCs (maps of content) for sub-topic clusters. An index file acts as an entry point that orients the agent to the landscape rather than a flat lookup table.

## Key Takeaways

- Single skill files work for simple tasks; domains with real depth need composable, linked skill graphs
- Progressive disclosure pattern (index → descriptions → links → sections → full content) minimizes token usage while preserving navigability
- Wikilinks embedded in prose carry semantic context — the agent understands *why* to follow a link, not just that a link exists
- YAML frontmatter on every node enables scan-without-read, so the agent routes based on descriptions rather than loading everything
- MOCs organize clusters of related skills into navigable sub-topics when graphs grow large
- The arscontexta plugin provides a ready-made skill graph for building knowledge systems; `/learn` and `/reduce` commands populate it

## Links

- [Article](https://x.com/i/article/2023918991673061376)
- [Original Tweet](https://x.com/arscontexta/status/2023957499183829467)
