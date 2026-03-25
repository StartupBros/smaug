---
title: "Self-Improving Skills for Agents"
type: article
date_added: 2026-03-12
source: "https://x.com/i/article/2032164771857059840"
author: "Vasilije (@tricalt)"
tags: [ai-agents, skills, self-improvement, cognee, agentic-systems]
via: "Twitter bookmark from @tricalt"
---

SKILL.md files are static while the environments around them constantly change. A skill that worked weeks ago can quietly start failing when codebases change, models behave differently, or user task patterns shift. The cognee-skills system (via the cognee Python library) proposes closing this feedback loop automatically.

## Key Takeaways

- **Static skills degrade silently**: Routing errors, failed tool calls, and underperforming instructions accumulate without any signal unless someone manually audits outputs
- **Observation is prerequisite**: Each skill execution logs what task was attempted, which skill was selected, whether it succeeded, what error occurred, and any user feedback — stored as a graph node via cognee's Custom DataPoint
- **Graph-structured storage**: Skills, runs, and feedback are stored as an interconnected graph, enabling tracing of recurring failure patterns across executions
- **`.amendify()` proposes changes**: Once failures accumulate, the system inspects the connected history and proposes targeted amendments — tightening triggers, reordering steps, adding missing conditions, or changing output formats
- **Evaluate before committing**: Amendments must prove measurable improvement before becoming the next skill version; the original instructions are never destroyed, making the process auditable and reversible
- **Full loop**: observe → inspect → amend → evaluate → update (or rollback)

## The Five-Stage Loop

1. **Ingestion** — Skills are indexed with semantic enrichment (summaries, task patterns, relationships) for better routing
2. **Observe** — Every execution appends a result node to the skill graph
3. **Inspect** — Accumulated failures trigger an analysis of the connected history to identify root causes
4. **Amend** — `.amendify()` generates a proposed patch grounded in execution evidence, reviewable by humans or applied automatically
5. **Evaluate & Update** — The amendment is tested; improvements are promoted, regressions are rolled back

## Links

- [Article](https://x.com/i/article/2032164771857059840)
- [cognee on PyPI](https://pypi.org/project/cognee/0.5.4.dev2/)
- [cognee on GitHub](https://github.com/topoteretes/cognee)
- [Original Tweet](https://x.com/tricalt/status/2032179887277060476)
