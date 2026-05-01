# mcpindex-ai

The agent-native index of [Model Context Protocol](https://modelcontextprotocol.io) servers.

Built for IDEs and agents that find the right MCP server at inference time — not the developer browsing a sidebar.

→ Live: **[mcpindex.ai](https://mcpindex.ai)**

## What's here

| Repo | What it is | License |
|------|-----------|---------|
| **[mcpindex-web](https://github.com/mcpindex-ai/mcpindex-web)** | The Next.js site, recommendation API, and quality scoring engine. 3,500+ MCP servers indexed daily from the official registry. | PolyForm NC 1.0.0 |
| **[mcp-server-mcpindex](https://github.com/mcpindex-ai/mcp-server-mcpindex)** | An MCP server for finding MCP servers. Drop-in for Claude Desktop, Cursor, Cline, Zed. | MIT |

## Three primitives

```bash
# Recommendation API — natural-language task -> top 3 servers
curl "https://mcpindex.ai/api/v1/recommend?task=read+pdfs+and+save+to+s3"

# Drop-in MCP server — install once, find the rest from inside your agent
npm install -g mcp-server-mcpindex

# Agent-readable surfaces
curl https://mcpindex.ai/llms.txt
curl https://mcpindex.ai/.well-known/mcp-index.json
```

## Quality scoring

Open methodology at [mcpindex.ai/methodology](https://mcpindex.ai/methodology). Five public-data signals — freshness, completeness, installability, documentation, semver stability — composited 0-100. PRs welcome.

## Affiliation

A personal research artifact, not a commercial product or service offering. Unofficial. Not affiliated with Anthropic. The Model Context Protocol is open under MIT and trademarks remain with their owners.

---

Written by [Gautam Bharti](https://github.com/gautamgb). More analysis at [seekgb.com](https://seekgb.com).
