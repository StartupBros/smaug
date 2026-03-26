---
title: "Claude Code Guide for Designers"
type: article
date_added: 2026-02-03
source: "https://x.com/i/article/2017852586888728578"
author: "Felix Lee (@felixleezd)"
tags: []
via: "Twitter bookmark from @felixleezd"
---

A step-by-step guide for designers who want to build and deploy web apps using Claude Code without prior coding experience. The author — a designer, not a developer — shares how he built a personal website with an AI chat widget and a growth design tool in under a week. The guide walks through installation, terminal basics, project scaffolding, iterative prompting, GitHub commits, Vercel deployment, custom domains, and integrating Supabase (auth + database) with OpenAI for AI-powered features. Key insight: designers already know how to give structured feedback, which maps directly to effective prompting. The guide emphasizes always starting with a planning prompt to generate a `plan.md` before writing any code.

## Key Takeaways

- Start every Claude Code project with a research/planning prompt that produces a `plan.md` file before any implementation begins
- Designers have a natural advantage: giving structured design feedback translates directly into effective AI prompting
- Full stack from zero: terminal → GitHub → Vercel → custom domain → Supabase auth → OpenAI integration is all achievable without writing code directly
- Use Supabase Edge Functions to store API keys server-side so they're never exposed to users
- The deploy loop (GitHub push → auto-deploy on Vercel) makes iteration extremely fast once set up
- Author built a Tetris game using Figma MCP → FigJam → Claude Code without touching a line of code manually

## Links

- [Article](https://x.com/i/article/2017852586888728578)
- [Original Tweet](https://x.com/felixleezd/status/2018728056249254377)
