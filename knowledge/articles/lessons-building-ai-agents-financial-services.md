---
title: "Lessons from Building AI Agents for Financial Services"
type: article
date_added: 2026-01-24
source: "https://x.com/i/article/2015173311903539200"
author: "Nicolas Bustamante (@nicbstme)"
tags: []
via: "Twitter bookmark from @nicbstme"
---

A practitioner's deep-dive from two years building Fintool, an AI agent platform for professional investors. The author (Nicolas Bustamante, Fintool CEO) argues that financial services is an especially demanding domain because professional investors make million-dollar decisions based on agent output and spot errors instantly. This forced extreme rigor: every number double-checked, every assumption validated. The article covers 11 architectural lessons learned, many involving infrastructure bets that felt contrarian at the time but proved correct.

**Core lessons:**

**Sandboxes are non-negotiable.** Each user gets an isolated execution environment with three S3 mount points (private R/W, org shared read-only, public read-only). AWS ABAC short-lived credentials scoped to S3 prefixes enforce isolation at the IAM level — not just application-level guards. Sandbox pre-warming (spinning up when the user starts typing) keeps latency invisible.

**Context is the product.** The real work is normalizing heterogeneous financial data (SEC filings, earnings transcripts, research PDFs, market data, 13Fs) into three formats: markdown for narrative, CSV/tables for structured data, JSON metadata for retrieval. Chunking strategy is domain-specific: 10-Ks chunk by regulatory section, earnings calls by speaker turn, news by paragraph.

**SEC parsing is adversarial.** Off-the-shelf parsers fail on nested tables, footnote cross-references, scanned exhibits, mixed units, and fiscal period ambiguity. Fintool maintains a fiscal calendar for 10,000+ companies to normalize "Q1 2024" — which means different date ranges for Apple vs Microsoft vs calendar year companies.

**Skills are the product, not the model.** Fintool adopted Anthropic's Agent Skills spec (markdown files with YAML frontmatter) as first-class citizens. A DCF skill encodes an analyst's complete methodology — step-by-step instructions, industry-specific guidelines, quality checks. Non-engineers write skills; no deployment needed; fully auditable. Copy-on-write shadowing lets users override shared skills with private versions.

**S3 beats databases for file storage.** User data lives in S3 rather than traditional databases. ReadFile, WriteFile, and Bash tools let the agent do genuine file-based workflows rather than in-memory transforms.

**Temporal for long-running tasks.** Temporal provides reliable execution with proper cancellation handling for multi-step agent workflows that span minutes.

**Evals are not optional.** Domain-specific evals catch errors before they reach professional investors. Production monitoring via a dedicated observability stack.

## Key Takeaways

- Isolated sandboxes with short-lived credentials are essential — not optional for production agent workflows
- Data normalization is 80% of the work; the agent quality ceiling is set by context quality, not model capability
- Skills (markdown files encoding domain methodology) are more valuable than prompt engineering — they're the actual product
- Fiscal period normalization requires a per-company calendar database; off-the-shelf date parsing fails at scale
- S3-first + filesystem tools enable richer workflows than API-only architectures
- The fear of being wrong in high-stakes domains becomes a feature — it drives the quality bar that generic tools can't match

## Links

- [Article](https://x.com/i/article/2015173311903539200)
- [Original Tweet](https://x.com/nicbstme/status/2015174818497437834)
