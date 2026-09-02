# Suggested Commands

- Install dependencies: `npm install`
- Run all unit tests: `npm test`
- Run one test file: `npx vitest run src/plugin/transform/model-resolver.test.ts`
- Typecheck: `npm run typecheck`
- Build publishable `dist/`: `npm run build`
- Model E2E smoke tests: `npm run test:e2e:models -- --model google/<model-id>`
- List Google models visible to OpenCode: `opencode models google`
- Generate config schema: `npm run build:schema`
- Check Serena memory references: `serena memories check`