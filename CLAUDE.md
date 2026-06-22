# CLAUDE.md

Guidance for Claude Code when working in this repo. This file is read automatically at the start of every session.

## Memory

Persistent rules and project context live in [docs/_memory/](docs/_memory/). **Read [docs/_memory/README.md](docs/_memory/README.md) at the start of work**, and follow the files it links:

- [docs/_memory/project-overview.md](docs/_memory/project-overview.md) — repo layout and intent.
- [docs/_memory/docs-style-guide.md](docs/_memory/docs-style-guide.md) — **mandatory** formatting rules for every file in `docs/`. Apply before creating or editing any doc.
- [docs/_memory/docs-template.md](docs/_memory/docs-template.md) — skeleton to start a new docs topic file.

## Repo layout

- `src/anvil` — Backend: Express + Postgres + TypeScript (ESM, pnpm).
- `src/orefield` — Frontend monorepo: pnpm workspaces (`apps/*`, `packages/*`).
- `docs/` — Knowledge base. All topic files must follow the docs style guide above.

## Conventions

- Use **pnpm** for all JS/TS work.
- Keep the BE (anvil) and FE (orefield) concerns separate.
- When writing docs, conform to [docs/_memory/docs-style-guide.md](docs/_memory/docs-style-guide.md) and start from the template.

## Restrictions

- **Never read `.env` files** (`.env`, `.env.*`) anywhere in the repo — not via the Read tool, not via `cat`/`grep`/`head`/etc. They hold secrets. If you need to know which variables exist, ask, or read a `.env.example` instead.
