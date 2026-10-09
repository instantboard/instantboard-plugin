# Instantboard

![Instantboard](plugins/instantboard/logo.svg)

Remote [MCP](https://modelcontextprotocol.io) server for [Instantboard](https://instantboard.app). Cursor, Codex, and Claude install the same plugin from this repository.

Server URL: `https://instantboard.app/mcp`

## Cursor

Cursor imports this repository as a marketplace. The plugin lives in `plugins/instantboard`.

In Cursor, open **Settings → Plugins → Add Marketplace** and import `instantboard/instantboard-plugin`. Complete Instantboard sign-in when Cursor asks.

You can also add the server directly:

```json
{
  "mcpServers": {
    "instantboard": {
      "url": "https://instantboard.app/mcp"
    }
  }
}
```

## Codex

```bash
codex plugin marketplace add instantboard/instantboard-plugin
codex plugin add instantboard@instantboard
```

Complete Instantboard sign-in when Codex asks.

## Claude

```bash
claude plugin marketplace add instantboard/instantboard-plugin
claude plugin install instantboard@instantboard
```

Complete Instantboard sign-in when Claude asks. Claude uses the same `.mcp.json` as Codex.

## License

MIT
