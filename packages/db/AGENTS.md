# @crm/db

Owns Prisma schema/migrations, shared client and persistence helpers. Keep DB access server-only; browser consumers must not import its barrels. Read [database notes](README.md#notes) and [root import rules](../../agent-notes.md). Generated auth models come from auth configuration; do not hand-edit them. Migration/reset/seed/deploy commands are outside this docs task.

Run commands from `packages/db/` with the owning workspace dependencies installed.

- `bun run check-types`: `tsc --noEmit`.
- `bun run lint`: `biome check .`.
- `bun run test`: `bun test`.
- `bun run build`: `prisma generate`.
