# Task Completion

For source changes, run in order:

1. Targeted Vitest files for touched modules.
2. `npm run typecheck`
3. `npm test`
4. `npm run build` so tracked/published `dist/` matches source.

For model routing changes, also inspect `opencode models google` and run the relevant `npm run test:e2e:models -- --model google/<model-id>` when credentials and upstream rollout permit. Report upstream/model availability failures separately from unit/build failures.