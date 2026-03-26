---
title: "Code Factory: How to setup your repo so your agent can auto write and review 100% of your code"
type: article
date_added: 2026-02-16
source: "https://x.com/i/article/2023001790258573312"
author: "Ryan Carson (@ryancarson)"
tags: []
via: "Twitter bookmark from @ryancarson"
---

A detailed engineering blueprint for building a fully automated agentic PR loop where a coding agent writes code, the repo enforces risk-aware checks before merge, and a code review agent validates the PR — all with machine-verifiable evidence. The system is designed so humans never need to be in the merge path for standard changes.

The pattern uses a single machine-readable contract (JSON) that defines risk tiers by file path, required checks per tier, docs drift rules, and evidence requirements for UI flows. A preflight `risk-policy-gate` runs before expensive CI jobs to avoid wasting compute on already-blocked PRs. The most critical lesson from running this in production: review state must be validated against the current PR head SHA — stale "clean" evidence from a previous commit can silently allow a bad merge.

The article also covers: deduplicating rerun requests with a single canonical bot (marker + SHA), an optional automated remediation loop where the coding agent patches its own review findings and pushes a fix commit, auto-resolving bot-only comment threads after a clean rerun, and requiring browser evidence manifests (not just screenshots) for UI/flow changes. Incidents get converted to harness test cases so regressions don't recur.

## Key Takeaways

- Store risk tiers, merge policy, and evidence requirements in a single JSON contract to eliminate silent drift
- Run `risk-policy-gate` before CI fanout — a blocked PR shouldn't waste CI minutes
- Validate review agent state against the exact current head SHA; stale approvals are a security hole
- Use one canonical rerun-comment workflow with SHA-based deduplication to prevent race conditions
- A remediation agent that reads review findings, patches code, and pushes to the branch can dramatically shorten the loop
- Auto-resolve only bot-only comment threads after a clean rerun; never touch human-participated threads
- Browser evidence must be structured assertions in CI artifacts, not manual screenshots
- Convert every production regression into a harness test case to build long-term coverage

## Links

- [Article](https://x.com/i/article/2023001790258573312)
- [Original Tweet](https://x.com/ryancarson/status/2023452909883609111)
