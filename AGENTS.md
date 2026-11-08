# crm instructions

Read [preserved upstream policies](agent-notes.md) before editing this scope.

Standing Oomor override: runtime provider keys, models and endpoints, and signup/signin policy, must be database-backed and admin-managed. Do not add environment configuration for them. Existing documented environment conventions are legacy implementation debt, not permission or a recommended pattern for new configuration; bootstrap environment is infrastructure-only. Preserve current implementation documentation and stronger local safety rules. This docs branch performs no runtime migration.

Bun/Turborepo CRM with app-specific backend/agent ownership.

Local commands: `bun run check-types`, `bun run lint`, `bun run test`, `bun run build`. Do not run DB deploy/reset/seed tasks. Read upstream docs for the touched area.

Oomor-only identity: kashik0i; origin must be oomor-hq/crm.
This branch changes docs only. No paid calls, production operations, public
signup changes, CI enabling or source refactors. Coordinator review before PR/merge.
