# api

Owns HTTP, auth, tRPC and mailbox sync. Enqueue durable `AgentTask` rows; research, enrichment, scoring and identity matching belong to apps/agent, not API fallbacks. Read [API policy](../../docs/api.md#intelligence-never-lives-in-the-api), including its documented exchange-rate exception.

Run commands from `apps/api/` with the owning workspace dependencies installed.

- `bun run check-types`: `tsc --noEmit`.
- `bun run lint`: `biome check .`.
- `bun run test`: `CRM_TELEMETRY_DISABLED=1 bun test --preload ./test/setup.ts`.
- `bun run build`: `bun build src/main.ts --target=bun --outdir dist --packages=external --sourcemap`.
