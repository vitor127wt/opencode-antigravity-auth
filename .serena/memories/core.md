# Project Core

- OpenCode plugin exporting `AntigravityCLIOAuthPlugin` / `GoogleOAuthPlugin` from `index.ts`; main orchestration is `src/plugin.ts`.
- Authenticates Google Antigravity OAuth, rotates accounts/quotas, transforms Gemini and Claude requests, and supports public Gemini API keys as fallback or primary routing.
- Model definitions and dynamic registry conversion live in `src/plugin/config/models.ts`; model/backend translation and thinking tiers live in `src/plugin/transform/model-resolver.ts`.
- Live public Gemini and Antigravity registries are cached by `src/plugin/model-catalog.ts`; request transforms are under `src/plugin/transform/` and API-key routing under `src/plugin/api-key.ts`.
- `dist/` is the published runtime output; source changes require `npm run build`.
- Detailed stack/tooling: `mem:tech_stack`. Project conventions: `mem:conventions`. Completion checks: `mem:task_completion`. Commands: `mem:suggested_commands`.