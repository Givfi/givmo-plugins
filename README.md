# Givmo plugins

Setup files for using Givmo from Claude Code, Codex and Cursor.

## Claude Code

In Claude Code, run:

```
/plugin marketplace add givfi/givmo-plugins
/plugin install givmo@givmo
```

To use your own Givmo account, run `/mcp` and sign in to Givmo.

## Codex

Add this table to your `~/.codex/config.toml`, keeping what is already there:

```toml
[mcp_servers.givmo]
url = "https://mcp.givmo.io/mcp"
```

Then restart Codex.

## Cursor

Add this to `~/.cursor/mcp.json` (every project) or to a project's
`.cursor/mcp.json`, keeping any servers already there:

```json
{
  "mcpServers": {
    "givmo": {
      "url": "https://mcp.givmo.io/mcp"
    }
  }
}
```

Then reload Cursor.
