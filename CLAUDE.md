# archcss

DSL for creating 2D architectural floor plans that compile to HTML + CSS.

## Stack

- TypeScript
- Custom tokenizer + AST parser (zero dependencies)
- Vitest + Playwright (testing)
- Bun workspaces (monorepo)

## Version

0.1.0-alpha.1

## Scripts

- `bun run dev` — Development server
- `bun run build` — Build packages
- `bun run test` — Unit tests (Vitest)
- `bun run test:visual` — Visual tests (Playwright)
- `bun run lint` — ESLint
- `bun run format` — Prettier
- `bun run release:alpha|beta|stable` — Release automation

## Packages

- `@archcss/parser` — Core parsing (~34KB)
- `@archcss/runtime` — DOM mounting
- `@archcss/postcss-plugin` — PostCSS integration
- `@archcss/vite-plugin` — Vite integration

## Key features

- Spatial positioning with grid units
- Rooms, walls, doors as DSL elements
- Repeat patterns
- Hierarchy markers (`@1`, `@2`, `@3`)
- Inline CSS support
- Config via `arch.config.json`
