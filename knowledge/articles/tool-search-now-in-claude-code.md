---
title: "Tool Search now in Claude Code"
type: article
date_added: 2026-01-14
source: "https://x.com/i/article/2011507229279825920"
author: "Thariq (trq212)"
tags: []
via: "Twitter bookmark from @trq212"
---

Anthropic announces MCP Tool Search for Claude Code — a dynamic tool-loading mechanism that activates when MCP tool descriptions would consume more than 10% of the context window. Previously, users with 7+ MCP servers could burn 67k+ tokens just on tool descriptions before any real work began; this resolves one of the most-requested GitHub issues (lazy loading for MCP servers). When triggered, Claude Code loads tools via search rather than preloading all of them, while still allowing normal preloaded behavior for lighter setups.

The announcement notes that the "server instructions" field becomes more useful with tool search enabled — it helps Claude know when to search for that server's tools, analogous to skills. MCP client developers are encouraged to implement the ToolSearchTool using their own custom search function. Programmatic tool calling (composing MCP tools via code) was explored but deprioritized in favor of shipping tool search first to address the context usage problem.

## Key Takeaways

- MCP Tool Search activates automatically when tool descriptions exceed 10% of context window
- Resolves the long-standing GitHub issue requesting lazy loading for MCP servers
- Users with 7+ MCP servers were consuming 67k+ tokens on tool descriptions alone
- The "server instructions" field gains importance as a routing hint for tool search
- MCP client developers should implement ToolSearchTool with a custom search function
- Programmatic MCP tool composition is still on the roadmap but deprioritized

## Links

- [Article](https://x.com/i/article/2011507229279825920)
- [Original Tweet](https://x.com/trq212/status/2011523109871108570)
