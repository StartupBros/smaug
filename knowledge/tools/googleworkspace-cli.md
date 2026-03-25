---
title: "googleworkspace/cli (gws)"
type: tool
date_added: 2026-03-04
source: "https://github.com/googleworkspace/cli"
tags: [cli, google-workspace, ai-agents, automation, rust, mcp]
via: "Twitter bookmark from @addyosmani"
---

A community-built Rust CLI (`gws`) that provides a single command-line interface for all of Google Workspace — Drive, Gmail, Calendar, Sheets, Docs, Chat, Admin, and more. Unlike static CLI tools, it dynamically generates its entire command surface at runtime by reading Google's Discovery Service, so new API endpoints are picked up automatically.

Designed for both human use and AI agent workflows, with structured JSON output and 40+ pre-built agent skills.

## Key Features

- **Dynamic command surface**: Reads Google Discovery Service at runtime — no static command list, always up to date
- **40+ agent skills**: Pre-built skills for AI agents to manage Workspace without custom tooling
- **Structured JSON output**: Every response is machine-readable, making it easy to pipe into LLMs or scripts
- **Auto-pagination**: `--page-all` streams paginated results as NDJSON
- **Dry-run mode**: Preview requests before executing with `--dry-run`
- **Schema introspection**: `gws schema <method>` reveals request/response schemas for any API method
- **Multiple auth methods**: OAuth, service accounts, pre-obtained tokens, `gcloud` integration
- **Cross-platform**: Available via npm, Homebrew, Nix, or pre-built binaries

## Install

```bash
npm install -g @googleworkspace/cli
# or
brew install googleworkspace-cli
```

## Links

- [GitHub](https://github.com/googleworkspace/cli)
- [Original Tweet](https://x.com/addyosmani/status/2029372736267805081)
