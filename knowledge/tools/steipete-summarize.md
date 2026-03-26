---
title: "summarize"
type: tool
date_added: 2026-02-02
source: "https://github.com/steipete/summarize"
tags: []
via: "Twitter bookmark from @arscontexta"
---

A CLI tool and Chrome/Firefox browser extension by Peter Steinberger (@steipete) that generates fast summaries of URLs, files, and media. It handles web pages, PDFs, YouTube videos, podcasts, audio/video files, and RSS — dispatching to transcript-first pipelines for media and falling back to Groq/Whisper/AssemblyAI/OpenAI when needed. The Chrome Side Panel mode adds a streaming chat interface with history, while the CLI supports JSON diagnostics, extract-only, and cost-estimate modes. With 5,000+ stars, it's a solid entry point for piping external content directly into an Obsidian vault or other PKM systems.

## Key Features

- CLI: summarize any URL, file, PDF, YouTube, or podcast in one command
- Chrome Side Panel + Firefox Sidebar with streaming Markdown chat and history
- YouTube slide extraction with OCR + timestamped cards
- Transcript-first media flow with multi-provider fallback (Groq, Whisper, AssemblyAI, Gemini, OpenAI, FAL)
- Supports local, paid, and free (OpenRouter) model presets
- Background daemon for browser extension streaming (launchd/systemd/Scheduled Task autostart)
- Output modes: Markdown, JSON diagnostics, extract-only, metrics, timing, cost estimates

## Links

- [GitHub](https://github.com/steipete/summarize)
- [Original Tweet](https://x.com/arscontexta/status/2018450512505627019)
