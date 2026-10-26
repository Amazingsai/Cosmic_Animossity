# Cosmic Animosity — Temporary AI Behavior Dataset

**Status: SYNTHETIC DEMONSTRATION DATA ONLY.** These 12 paired examples were authored as illustrative placeholders. They are **not** outputs recorded from an LLM, not gameplay observations, and not evidence of improved AI performance. Do not report them as experimental results.

## Layout
- `inputs/`: 12 JSON prompts describing desired enemy behavior.
- `outputs/`: 12 matching JSON rule sets, with the same `id` as each input.
- `manifest.csv`: index of all pairs.

## Interpretation
The `rules` are human-readable pseudologic for planning Unreal Engine Blueprints, **not** a native Unreal Engine Behavior Tree or directly executable JSON. The `decision_policy` is `first_matching_rule`, so rule priority matters. Conditions refer to hypothetical game variables; some features (such as projectile detection, attack cooldowns, and last known position) may not exist in the current game and would need to be implemented. Distance thresholds are illustrative Unreal units.

## Later replacement
For a real experiment, save actual prompt text, model name/version, generation settings, raw LLM response, parsed/validated behavior, Unreal implementation, trial conditions, and measured gameplay outcomes. Keep real observations in a separate, clearly labeled dataset.
