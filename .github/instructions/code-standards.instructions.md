---
description: 'Comment philosophy and TypeScript formatting standards'
applyTo: '**/*.{ts,astro,css}'
---

# Code Comment and TypeScript Style

## Comments and documentation

- Explain **why** code exists or why a non-obvious decision was made; do not narrate mechanics or restate what the code already says.
- Keep comments concise and close to the code they explain. Remove comments that add no context.
- Treat stale comments and documentation as bugs. Update or remove them in the same change as the related code.
- Use TSDoc for exported functions in `db/` and `src/lib/`, following [`drizzle.instructions.md`](drizzle.instructions.md).
- Document reusable Astro component `Props` interfaces so their public API is clear, following [`astro.instructions.md`](astro.instructions.md).

## TypeScript formatting

- In application `.ts` files, indent with four spaces; do not use tabs. Playwright specs in `e2e-tests/` and `playwright.config.ts` use two spaces.
- In `.ts` files, use single quotes for strings unless escaping would be required.
- In `.ts` files, end statements with semicolons.
- Keep explicit parameter and return types on functions, especially in `db/` and `src/lib/`.
- ESLint enforces indentation, quote style, and semicolons in `.ts` files. Follow the existing rules rather than adding local formatting exceptions.
