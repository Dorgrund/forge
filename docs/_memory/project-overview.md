# Project Overview

ForgeOfDorgrund is the user's personal initiative to build and eventually ship apps to real users. The repo has three top-level concerns:

- `src/anvil` — **Backend.** Express + Postgres (`pg`) + TypeScript, ESM, pnpm. Dev via `tsx watch src/server.ts`; build via `tsc`; has `docker-compose.yml` and `scripts/migrate.ts` (`pnpm db:migrate`). CI = `lint && typecheck`.
- `src/orefield` — **Frontend monorepo.** pnpm workspaces under `apps/*` and `packages/*`. Apps: `waterTracker`, `englishWords`, `moneyTracker` (started via `pnpm start:<app>`). CI = `lint && typecheck` (`pnpm -r`).
- `docs/` — Knowledge base of investigations, approaches, and quality practices for building the apps. Every file added must follow [docs-style-guide.md](docs-style-guide.md) and start from [docs-template.md](docs-template.md).

**Why:** This is a long-term, quality-focused personal project, not a throwaway. Docs capture durable, high-quality engineering approaches.

**How to apply:** When asked to write docs, always conform to the style guide and template. When working in code, respect the BE (anvil) vs FE (orefield) split and use pnpm.
