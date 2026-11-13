# Installing Timefire

Timefire is a hosted, read-only MCP server. There is nothing to clone, build or install, and it needs no API key or account.

- URL: `https://api.timefire.ai/mcp/`
- Transport: Streamable HTTP

## Cline

Add this entry to `cline_mcp_settings.json`:

```json
{
  "mcpServers": {
    "timefire": {
      "type": "streamableHttp",
      "url": "https://api.timefire.ai/mcp/"
    }
  }
}
```

Or in the Cline panel: MCP Servers, then Remote Servers. Name it Timefire, paste `https://api.timefire.ai/mcp/`, set Transport Type to Streamable HTTP, and click Add Server.

## Check it works

Ask: "Using Timefire, list the graded books." The `list_resolved_batches` tool should return recent books.

Setup steps for other clients: https://timefire.ai/developers/mcp/
