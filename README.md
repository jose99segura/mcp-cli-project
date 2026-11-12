# MCP CLI Project

Playground for building an MCP server and client (document-chat CLI).

- `starter/` — your working copy. Implement the TODOs in `mcp_server.py` and `mcp_client.py`.
- `complete/` — reference solution. Use it to compare or unblock yourself.

## Setup

1. In `starter/` (and `complete/` if you want to run the reference), copy `.env.example` to `.env`
   and set your Anthropic API key: `ANTHROPIC_API_KEY="sk-ant-..."`
2. Install dependencies in each folder: `uv sync`

## Run

```bash
cd starter
uv run main.py
```

- `@doc_id` mentions a document (e.g. `Tell me about @deposition.md`)
- `/prompt doc_id` runs a server prompt (e.g. `/format plan.md`), Tab to autocomplete

Test the server alone with the MCP Inspector:

```bash
uv run mcp dev mcp_server.py
```
