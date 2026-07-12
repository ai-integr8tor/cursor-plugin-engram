---
name: local-recall
description: Search and store self-hosted conversation memory through the Local Recall MCP server
---

Use the Local Recall MCP tools to recover relevant prior context and preserve durable outcomes.

Search first when prior work may matter:

```text
search query="$ARGUMENTS" limit=5
```

After meaningful work, create a conversation and append the essential request, outcome, and reasoning. Skip routine operations and never store credentials. If the user asks to remove memory, use `delete_conversation` and report the result.
