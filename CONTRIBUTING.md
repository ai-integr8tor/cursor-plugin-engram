# Contributing

Keep this repository a thin Cursor adapter over standard MCP.

- Put memory behavior and protocol changes in the Local Recall core first.
- Keep hosted services optional and explicit; do not add silent fallbacks.
- Do not commit credentials or memory data.
- Preserve the original MIT copyright and attribution notice.
- Validate JSON files before proposing changes.

Other IDE integrations should reuse the same MCP contract rather than fork the memory engine.
