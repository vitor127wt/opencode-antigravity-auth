# Tech Stack

- TypeScript ESM, Node.js >=20, strict compiler options with bundler module resolution.
- OpenCode plugin API: `@opencode-ai/plugin`.
- Validation/config: Zod 4; OAuth: `@openauthjs/openauth`; account-file locking: `proper-lockfile`.
- Tests: Vitest 3 in Node environment; test files are `src/**/*.test.ts`.
- Build/typecheck: TypeScript 5.9; `tsconfig.build.json` emits JS, declarations, and source maps to `dist/`.
- npm scripts are authoritative; package manager metadata present in `package-lock.json`.