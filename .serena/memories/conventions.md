# Conventions

- Prefer small extensions of existing model-family logic over parallel routing paths.
- Static OpenCode model metadata belongs in `OPENCODE_MODEL_DEFINITIONS`; dynamically discovered model metadata must merge without discarding curated static fields.
- Keep public Gemini IDs, Antigravity-facing IDs, and backend IDs distinct. Confirm Antigravity IDs against `v1internal:fetchAvailableModels`; backend naming is not reliably derivable from public names.
- Gemini 3 thinking variants use `thinkingLevel`; Claude extended thinking variants use token budgets.
- Public/Gemini CLI dotted-minor Gemini 3 IDs use bare names; legacy Gemini 3.0 uses `-preview`.
- Newer Gemini models that reject sampling controls must be covered by `sanitizeGeminiGenerationConfigForModel` and expose `temperature: false`.
- Tests use Vitest globals and generally colocate with implementation. Source style is ESM imports, explicit exported types, double quotes, two-space indentation, and trailing commas.