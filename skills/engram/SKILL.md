---
name: engram
description: Search and store memories in Engram for persistent context across sessions
---

Use the Engram MCP server to manage persistent memory.

## Search for relevant context

When starting a task or needing prior context, search Engram:

```
search query="$ARGUMENTS" limit=5
```

Review the results and incorporate relevant context into your working memory.

## Store important context

After completing significant work, create a conversation and append messages:

```
create_conversation title="<concise title>" agent_id="cursor" tags=["<tag1>", "<tag2>"]
```

Then append the key details:

```
append_messages conversation_id="<id>" messages=[{"role": "user", "content": "<what was asked>"}, {"role": "assistant", "content": "<what was done>"}]
```

Store decisions, bug fixes, architecture choices, and user preferences. Skip routine operations.
