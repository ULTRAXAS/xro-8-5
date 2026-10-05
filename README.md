# Search 5

Grok Build plugin for **Search 5** by ULTRAXAS — live web search with citations and Xro chat, backed by the public MCP server at [https://ai.ultraxas.com/mcp](https://ai.ultraxas.com/mcp).

This is a thin wrapper (same pattern as Sentry and Vercel): it does not run a local server. It points Grok Build at the hosted MCP (`web_search` and `chat`).

## Install

Once listed in the [xAI plugin marketplace](https://github.com/xai-org/plugin-marketplace):

```bash
grok plugin install search-5 --trust
```

Or browse in Grok Build with `/marketplace`, find **Search 5**, and press `i`.

## Manual MCP (without the marketplace)

```bash
grok mcp add --transport http search-5 https://ai.ultraxas.com/mcp
```

## Requirements

- Grok Build CLI
- Public HTTPS reachability to `https://ai.ultraxas.com/mcp` (no auth required today)

## What you get

| Tool | Purpose |
|------|---------|
| `web_search` | Live web search with a synthesized answer and source citations |
| `chat` | Message the ULTRAXAS Xro chat model |

## Links

- MCP endpoint: https://ai.ultraxas.com/mcp
- Site: https://ultraxas.com
- Marketplace (submit via PR): https://github.com/xai-org/plugin-marketplace

## License

MIT — see [LICENSE](LICENSE).
