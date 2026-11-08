# @crm/telemetry

Owns server telemetry event builders, property allowlist and install identity. Read [telemetry policy](../../docs/telemetry.md) before adding events/properties. Never send CRM row values, secrets or user identity; preserve allowlisting and opt-out (`CRM_TELEMETRY_DISABLED=1` or `DO_NOT_TRACK=1`). Tests must emit nothing; preserve the API/agent test-script opt-out. Landing analytics has a separate hostname-gated policy; do not expand it to CRM pages.

Run commands from `packages/telemetry/` with the owning workspace dependencies installed.

- `bun run check-types`: `tsc --noEmit`.
- `bun run lint`: `biome check .`.
- `bun run test`: `bun test`.
