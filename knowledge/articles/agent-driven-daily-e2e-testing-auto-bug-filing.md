---
title: "How to setup your agent to do daily testing + file bugs"
type: article
date_added: 2026-02-02
source: "https://x.com/i/article/2017713291540267008"
author: "Ryan Carson"
tags: []
via: "Twitter bookmark from @ryancarson"
---

A practical guide to running a daily agent-driven end-to-end test suite that catches regressions and auto-files bugs before the team starts work. The approach differs from traditional Playwright/Cypress CI testing: instead of brittle CSS selectors and mocked auth, it uses accessibility tree semantic snapshots (via `agent-browser`) and runs daily as a safety net—not as a PR gate.

The system runs at 9 AM via macOS launchd, performs a full fresh-user signup (deleting the test user from DB, Clerk/auth provider, and Stripe/payment provider first), handles Google OAuth unattended via a pre-signed Chrome debug profile, flows through onboarding using pattern-matched responses to the AI's messages, tests key feature tools, and on failure generates a report and creates a ticket in the issue tracker automatically.

Key implementation details: the `delete-test-user.ts` cleanup script must use dotenv's `-o` flag to override `.env.local` with production env; retry logic runs up to 2 attempts with 5-second sleep; bug deduplication checks for similar tickets in the last 24 hours before creating new ones; artifacts (logs, screenshots) retained for 7 days. Security: the Chrome debug profile contains live session tokens and must be treated like production SSH keys—never commit, never run on shared machines, use a dedicated test Google account.

The core insight: your AI agent already knows how to interact with your app. Give it a script, a schedule, and an issue tracker API—and you have autonomous QA.

## Key Takeaways

- Agent-driven E2E uses semantic accessibility tree snapshots—adapts to UI changes that break CSS selector tests
- Pre-signed Chrome debug profile enables fully unattended Google OAuth without mocking
- Full cleanup (DB + auth + payments) before each run guarantees a clean slate and catches cross-system consistency bugs
- Automatic bug filing with deduplication prevents alert fatigue from flaky runs
- Best for apps with AI/chat flows or complex OAuth; not a replacement for deterministic Playwright CI gating
- launchd scheduling (macOS) or GitHub Actions with `storageState` for CI environments

## Links

- [Article](https://x.com/i/article/2017713291540267008)
- [Original Tweet](https://x.com/ryancarson/status/2018354837918732297)
