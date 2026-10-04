# Twelfth MCP

[![smithery badge](https://smithery.ai/badge/twelfth/twelfth)](https://smithery.ai/servers/twelfth/twelfth)
[![Twelfth MCP connector – tool definition quality and endpoint health on Glama](https://glama.ai/mcp/connectors/ai.twelfth/workspace/badges/score.svg)](https://glama.ai/mcp/connectors/ai.twelfth/workspace)

Connect an AI assistant to your [Twelfth](https://twelfth.ai) workspace.

Twelfth is a commercial workspace for retail and category teams. Its hosted MCP
server lets Cursor, Claude, ChatGPT and other MCP clients read the products,
suppliers, sales, inventory, pricing, projects, members and actions that your
Twelfth account can access.

- **Endpoint:** `https://api.twelfth.ai/mcp` (Streamable HTTP)
- **Auth:** OAuth 2.1. Sign in with your Twelfth account, choose a workspace,
  and approve the read tools you want. Revoke any time from
  **Settings → AI & agents**.
- **Read-only.** Every tool reads; nothing writes back to Twelfth.
- **Official MCP Registry:** [`ai.twelfth/workspace`](https://registry.modelcontextprotocol.io/v0.1/servers?search=ai.twelfth/workspace&version=latest)
- **Docs:** https://twelfth.ai/developers/mcp

You need a Twelfth workspace to connect. [Book a demo](https://twelfth.ai/book-a-demo)
if your team doesn't have one yet.

## Install

### Cursor

Install **Twelfth** from the Cursor Marketplace, or add it to `.cursor/mcp.json`:

```json
{
  "mcpServers": {
    "twelfth": { "url": "https://api.twelfth.ai/mcp" }
  }
}
```

### Claude Code

```sh
/plugin marketplace add twelfth-ai/twelfth-mcp
/plugin install twelfth@twelfth
```

Or just the server: `claude mcp add --transport http twelfth https://api.twelfth.ai/mcp`

### Claude, ChatGPT and other clients

Add a custom connector with the URL `https://api.twelfth.ai/mcp` and complete
the Twelfth sign-in.

## What's in this repo

This repository holds client configuration only; the server is hosted by
Twelfth.

| Path | What |
| --- | --- |
| `plugins/twelfth/` | The plugin: MCP config for Cursor (`mcp.json`) and Claude Code (`.mcp.json`), and a `twelfth-workspace` skill that helps the assistant use the tools well |
| `.cursor-plugin/`, `.claude-plugin/` | Marketplace manifests for Cursor and Claude Code |

## Support and security

- Questions: hello@twelfth.ai
- Security reports: https://twelfth.ai/.well-known/security.txt
- Privacy: https://twelfth.ai/legals/privacy

The contents of this repository are MIT licensed. The Twelfth service is
governed by its [terms](https://twelfth.ai/legals/terms).

smithery-verification=0c586824f907c08ca5140641c9ddc0c07e5e1574fd305497c14360c7f4ded531
