# api

Run from this directory with the owning workspace dependencies installed.

- `bun run check-types`: `tsc --noEmit`.
- `bun run lint`: `biome check .`.
- `bun run test`: `CRM_TELEMETRY_DISABLED=1 bun test --preload ./test/setup.ts`.
- `bun run build`: `bun build src/main.ts --target=bun --outdir dist --packages=external --sourcemap`.
