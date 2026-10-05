# xro-search

Grok Build plugin for **ULTRAXAS Xro** — live web search with citations and Xro chat, backed by the public MCP server at [https://ai.ultraxas.com/mcp](https://ai.ultraxas.com/mcp).

This is a thin wrapper (same pattern as Sentry and Vercel): it does not run a local server. It points Grok Build at the hosted `xro-search` MCP (`web_search` and `chat`).

## Install

Once listed in the [xAI plugin marketplace](https://github.com/xai-org/plugin-marketplace):

```bash
grok plugin install xro-search --trust
```

Or browse in Grok Build with `/marketplace`, find **xro-search**, and press `i`.

## Manual MCP (without the marketplace)

```bash
grok mcp add --transport http xro-search https://ai.ultraxas.com/mcp
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
