# Nutcracker Agentic Specification

This repository hosts the **public agentic specification** for the Nutcracker SaaS platform.

It contains:
- `agent-schema.json` — global agentic schema
- `manifest.json` — global MCP manifest
- `VERSION` — current schema version
- `CHANGELOG.md` — version history

These files are referenced by:
- `/.well-known/mcp.json`
- `/ai/agent-schema.json`
- `/ai/manifest.json`

Tenant-specific MCP manifests remain served from:
`https://nutcrackerbot.com/api/{tenant_id}/mcp/manifest.json`

This repository is public so that AI agents can:
- discover Nutcracker’s agentic interface
- validate schema versions
- generate correct tool calls
- operate safely under agentic_scope

Backend code remains private in the `nutcracker-backend` repository.
Console code remains public in the `nutcracker-console` repository.