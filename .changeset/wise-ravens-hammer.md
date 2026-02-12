---
"@marckrenn/pi-sub-bar": patch
"@marckrenn/pi-sub-core": patch
---

- Sub-core Codex provider now parses `additional_rate_limits` from the usage API response and exposes them as additional usage windows, enabling model-specific quotas like **GPT-5.3 Codex Spark** to be tracked.
- Sub-bar now filters Codex usage windows so `GPT-5.3-Codex-Spark` usage is shown only when that model is the selected model; other Codex models show only standard Codex usage windows.
