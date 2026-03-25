---
title: "QMD - Query Markup Documents"
type: tool
date_added: 2026-03-25
source: "https://github.com/tobi/qmd"
tags: [search, markdown, ai-agents, knowledge-base, local-search]
via: "Twitter bookmark from @nurijanian"
---

QMD is an on-device search engine for markdown files, built by Shopify CEO Tobi Lütke. It combines multiple search approaches running entirely locally: BM25 full-text retrieval, vector semantic search via a locally-running 300MB embedding model, and LLM re-ranking for final relevance scoring.

Perfect for PM workflows and agentic AI systems. Index markdown notes, meeting transcripts, documentation, and knowledge bases. Search with keywords or natural language entirely offline—no data leaves your machine.

## Key Features

- **Hybrid Search**: BM25 keyword search + vector semantic search + LLM re-ranking
- **Local Processing**: All indexing and searching happens on your machine
- **Context Trees**: Add contextual metadata to help LLMs make better document selections
- **Multiple Output Modes**: JSON, files, structured results for agentic workflows
- **MCP Server Support**: Integrated with Claude Desktop and Claude Code via Model Context Protocol
- **Flexible Installation**: Works with Node.js, Bun, or run directly via npx/bunx
- **API/SDK**: Available as a library for Node.js and Bun applications

## Use Cases

- **PM Workflow**: Quickly search product decision history, research notes, and meeting transcripts without manual copying
- **Agentic AI**: Provide agents with structured access to your knowledge base for context-aware responses
- **Knowledge Management**: Maintain searchable Obsidian vault or markdown documentation
- **Session Context**: Feed Claude Code relevant prior work before starting new sessions

## Links

- [GitHub](https://github.com/tobi/qmd)
- [Original Tweet](https://x.com/nurijanian/status/2032124503330058696)
