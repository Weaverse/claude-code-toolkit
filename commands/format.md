---
description: Auto-format code and fix TypeScript issues
---

# Auto Format Code

I'll format your code and fix TypeScript issues using the project's configured tools.

I'll detect and run:
- **Formatters**: Prettier, ESLint --fix, Biome, rustfmt, black, etc.
- **TypeScript fixes**: eslint --fix, tsc --noEmit for type checking
- **Import fixes**: organize imports, remove unused imports

Process:
1. Check for config files (prettier.config.js, .eslintrc, tsconfig.json)
2. Run formatters on modified files first
3. Fix TypeScript errors and warnings
4. Show summary of changes made

Commands I'll try:
- `nr biome:fix` (primary - formats and fixes TypeScript)
- `npm run format` or `yarn format`
- `tsc --noEmit` for type checking

Fast, focused formatting with TypeScript error resolution.