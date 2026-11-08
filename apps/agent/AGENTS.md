# agent

Owns intelligence, vendor clients, confidence decisions and agent task execution. The API enqueues tasks; this service leases and executes them. Read [agent policy](../../docs/agent.md) and the installed version of eve docs before changing tools or dispatch. Preserve task budgets and capability gating; no live provider calls on this docs task.

Run commands from `apps/agent/` with the owning workspace dependencies installed.

- `bun run check-types`: `tsc --noEmit`.
- `bun run lint`: `biome check .`.
- `bun run test`: `CRM_TELEMETRY_DISABLED=1 bun test`.
- `bun run build`: `eve build`.
