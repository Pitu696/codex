# Contributing to Codex CLI

This document summarizes the development workflow and how to run the quality checks locally.

## Development workflow

- Create a topic branch from `main` (for example `feat/your-change`).
- Keep changes focused and prefer small pull requests.
- Use `pnpm test:watch` while iterating for fast feedback.
- We rely on **Vitest** for unit tests, **ESLint** and **Prettier** for style, and **TypeScript** for type-checking.
- Before pushing, run the complete suite:

```bash
pnpm test && pnpm run lint && pnpm run typecheck
```

Additional helpful commands:

```bash
# Watch mode (tests rerun on change)
pnpm test:watch

# Type-check without emitting files
pnpm typecheck

# Automatically fix lint and formatting issues
pnpm lint:fix
pnpm format:fix
```

Git hooks powered by [Husky](https://typicode.github.io/husky/) automatically run lint-staged on commit and execute tests and type checking on push.

## Contributor License Agreement

All contributors **must** accept the CLA.
Add a comment to your pull request with the text below:

```
I have read the CLA Document and I hereby sign the CLA
```

The CLA-Assistant bot will mark the status check as passed once every author has signed.
