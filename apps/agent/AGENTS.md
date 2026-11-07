# agent

Run from this directory with the owning workspace dependencies installed.

- `bun run check-types`: `tsc --noEmit`.
- `bun run lint`: `biome check .`.
- `bun run test`: `CRM_TELEMETRY_DISABLED=1 bun test`.
- `bun run build`: `eve build`.
