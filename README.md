# Local Recall adapter for Cursor

This repository is a small, MIT-licensed adapter that connects Cursor to the self-hosted [Local Recall core](https://github.com/ai-integr8tor/engram) through standard MCP.

It intentionally contains no memory engine, hosted-service dependency, account system, or IDE-specific fork of the core. Other editors can use the same stdio or Streamable HTTP interfaces documented by the core repository.

## Setup

1. Build or install the `local-recall` binary from `ai-integr8tor/engram`.
2. Make the binary available on `PATH`.
3. Set `LOCAL_RECALL_DATA_PATH` to an operator-controlled data file.
4. Optionally set `LOCAL_RECALL_WORKSPACE`; it defaults to `default`.
5. Install this plugin or copy `mcp.json`, `rules/`, and `skills/` into the equivalent Cursor configuration.

The adapter launches:

```text
local-recall mcp
```

No API key or hosted Engram account is required.

## Public tools

- `create_conversation`
- `append_messages`
- `search`
- `get_conversation`
- `list_conversations`
- `delete_conversation`

## Extending it

Keep marketplace metadata, editor prompts, and presentation here. Add memory behavior to the core MCP/OpenAPI contract first so Cursor, VS Code, Codex, mobile clients, and future integrations stay compatible.

This adapter is not affiliated with Get Engram LLC. The original MIT copyright notice remains in `LICENSE` because this repository began from their public Cursor adapter.
