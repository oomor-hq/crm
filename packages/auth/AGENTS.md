# @crm/auth

Owns Better Auth configuration, sessions and authorization helpers; server auth and DB-backed exports stay server-only. Browser code must use the dedicated client export, never a server barrel. Read [auth topology](README.md#topology) and [root import rules](../../agent-notes.md). Existing signin env documentation is legacy debt under the root DB/admin override; auth generation rewrites the DB schema and is outside this docs task.

Run commands from `packages/auth/` with the owning workspace dependencies installed.

- `bun run check-types`: `tsc --noEmit`.
- `bun run lint`: `biome check .`.
- `bun run test`: `bun test`.
