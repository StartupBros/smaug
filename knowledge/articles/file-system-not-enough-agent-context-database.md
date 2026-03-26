---
title: "a file system is not all you need"
type: article
date_added: 2026-03-12
source: "https://x.com/i/article/2031876610975285249"
author: "Regina Lin"
tags: []
via: "Twitter bookmark from @reggitales"
---

A counterargument to the popular "markdown files as the best primitive for agent context" trend. The author argues that markdown file graphs are secretly reinventing databases in the worst possible substrate: the moment you need to query across your graph (e.g., find all decisions that contradict the current roadmap), you're doing full-text search across thousands of files. A real database gives you joins, indexes, constraints, and dependency tracking — a folder tree gives you grep.

The deeper problem is provenance and maintenance. When a source of truth (a Google Doc, a Slack message) updates, a derived markdown note becomes stale with no mechanism to cascade the update. A database can store references to original sources, track what was derived from what, and propagate changes automatically. The article also challenges the "code analogy" — code is executable and self-verifying through tests; company context has no equivalent truth-maintenance mechanism, so a beautiful graph traversal can still produce confidently wrong results.

The proposed architecture: work apps (Drive, Slack, CRM, Linear) as source of truth → a file layer for agent instructions, SOPs, and scratchpad → a database layer for extracted information, typed relationships, dependency chains, and provenance pointers. This lets agents query a live structured graph rather than grepping a folder tree, and enables cascading updates when sources change.

## Key Takeaways

- Markdown file graphs are functionally schemas with no enforcement — you've built a database but hidden the complexity inside folder trees
- The maintenance problem isn't solved by "agents don't get bored" — the structural issue is two copies of information that drift when the original source changes
- The code analogy breaks down because company context isn't executable and has no self-verification; traversal is not truth maintenance
- Flat text loses critical metadata: is this authoritative or speculative? Current or stale? Binding or one person's framing?
- The winning architecture separates hot-access file metadata from a structured database layer with provenance tracking and dependency chains
- Organizations that accumulate compounding context (structured, pointer-based, provenance-aware) will outpace those with better notes or wikis

## Links

- [Article](https://x.com/i/article/2031876610975285249)
- [Original Tweet](https://x.com/reggitales/status/2031916056760201714)
