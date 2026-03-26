---
title: "Your Company is a Filesystem"
type: article
date_added: 2026-02-10
source: "https://x.com/i/article/2021308996020211712"
author: "Eli Mernit"
tags: []
via: "Twitter bookmark from @mernit"
---

Mernit argues that OpenClaw's core insight — using a local filesystem as the agent's persistent state — is a model that scales directly to entire companies. Just as OpenClaw reads and writes files to remember context, a business could be modeled as a directory tree: `/cases`, `/billing/time-sheet`, `/clients`. The filesystem then becomes the shared namespace that agents need to access all relevant data, solving the enterprise problem of data siloed across Quickbooks, Outlook, Sharepoint, and Netsuite.

Two properties make this compelling: (1) unix file permissions map naturally to organizational hierarchy (first-year associates get read/write on their own folders, partners get access to everyone's), and (2) the entire back-office operation becomes a state machine. The article reduces AI agent architecture to two components — filesystem as state, Claude as orchestrator — and proposes that this pairing is powerful enough to run a law firm, a logistics operation, or any data-intensive business.

## Key Takeaways

- Modeling a company as a filesystem gives AI agents a single, unified namespace to read and write — eliminating data silo problems
- Unix file permissions double as org-chart governance with no additional tooling
- The filesystem-as-state pattern scales from personal OpenClaw use to enterprise agent deployment
- Full company operations (case assignment, billing, client records) can be expressed as file reads and writes on a shared volume

## Links

- [Article](https://x.com/i/article/2021308996020211712)
- [Original Tweet](https://x.com/mernit/status/2021324284875153544)
