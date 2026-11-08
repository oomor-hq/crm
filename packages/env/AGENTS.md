# @crm/env

Owns repo-root environment loading, not runtime product configuration. Read [environment implementation](../../docs/environment.md) subject to the [root standing override](../../AGENTS.md): existing provider and signin/signup environment conventions are legacy debt; do not extend them or add per-package env files.

Run commands from `packages/env/` with the owning workspace dependencies installed.

- `bun run check-types`: `tsc --noEmit`.
- `bun run lint`: `biome check .`.
- `bun run test`: `bun test`.
