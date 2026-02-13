---
"@marckrenn/pi-sub-bar": minor
"@marckrenn/pi-sub-core": minor
"@marckrenn/pi-sub-shared": minor
---

- [#10](https://github.com/marckrenn/pi-sub/pull/10) defaults `showContextBar` to off for upgrades and new installs, so the context bar is hidden unless enabled explicitly. Thanks [@pasky](https://github.com/pasky) for this feature.
- Added optional context-window usage rendering: when enabled, an optional `Ctx` bar can be shown as the leftmost window and context-aware bar placement support was added for status display.
- Sub-core now supports parsing Codex `additional_rate_limits` and exposes model-specific Spark quotas; sub-bar now filters and formats Codex Spark usage windows for model-specific models, including `Codex (Spark)` provider labeling.
- Fixed tool registration compatibility with the latest Pi tool API by updating the `execute` callback parameter order in `sub-core` tool handlers (aligning with upstream `ExtensionAPI` typing).
