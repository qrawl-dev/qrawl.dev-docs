# qrawl-docs

Documentation site for **qrawl.dev**, built with [Mintlify](https://mintlify.com), deployed at docs.qrawl.dev.

Public repo so Google can index it and the community can PR doc fixes.

Planned structure:

- **Quickstart** — 5-minute key-to-first-crawl walkthrough
- **API Reference** — every endpoint with request/response examples
- **SDKs** — Node (`qrawl`) and Python (`qrawl-py`, imported as `qrawl`)
- **MCP setup** — config for Claude Desktop, Cursor, Windsurf, VS Code
- **Integrations** — LangChain, LlamaIndex, OpenAI tools
- **Self-hosting** — `docker compose up` with the OSS engine
- **Webhooks & signatures** — HMAC verification guide

| | |
|---|---|
| **Domain** | docs.qrawl.dev |
| **Visibility** | Public |
| **Infra** | Mintlify hosting |

## Local development

```bash
npm i -g mint   # Mintlify CLI
mint dev        # preview at http://localhost:3000
```

Configuration lives in `docs.json`; pages are `.mdx` files. Current structure: Get started
(Introduction, Quickstart, Self-hosting), SDKs (Node, Python), Integrations (MCP, frameworks),
and the API reference (auth, errors, scrape/crawl/map).
