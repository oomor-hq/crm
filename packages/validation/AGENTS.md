# @crm/validation

Owns schemas for stored JSON and payloads crossing package/process boundaries. Parse unknown input once at entry; export schema-derived types by subpath, describe actual stored shapes and report parse failures instead of empty fallbacks. See [boundary policy](../../agent-notes.md#parse-at-the-boundary-never-pass-recordstring-unknown-around) and [agent-manifest source](src/agent-manifest.ts).

Run commands from `packages/validation/` with the owning workspace dependencies installed.

- `bun run check-types`: `tsc --noEmit`.
- `bun run lint`: `biome check .`.
- `bun run test`: `bun test`.
