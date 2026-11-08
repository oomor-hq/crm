# @crm/mcp-integrations

Owns shared integration vendor/catalog, access modes, scope and tool contracts ([catalog source](src/catalog.ts)); keep these consistent across API and agent consumers. Connections expose capabilities, while automations belong to the agent builder: read [connections policy](../../docs/connections.md). Connection removal requires server-side owner/admin authorization, not merely a session.

Run commands from `packages/mcp-integrations/` with the owning workspace dependencies installed.

- `bun run check-types`: `tsc --noEmit`.
- `bun run lint`: `biome check .`.
- `bun run test`: `bun test`.
