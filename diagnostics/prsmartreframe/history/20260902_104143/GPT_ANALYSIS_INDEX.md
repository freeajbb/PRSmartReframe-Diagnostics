# GPT Analysis Bridge

- App: `PRSmartReframe 0.4.11`
- Goal: avoid deep GitHub blob traversal/cache misses.
- Start with `manifest.json`, then read the single shallow `GPT_ANALYSIS_BUNDLE.json`.
- For visual QA, inspect the shallow contact sheets below; each panel is labeled with the result ordinal and frame role.

## Shallow analysis artifacts

- `GPT_ANALYSIS_BUNDLE.json` — sanitized runtime state + desktop log + batch JSON + all pose result JSONs
- `GPT_OVERLAY_CONTACT_SHEET_EARLY.jpg`
- `GPT_OVERLAY_CONTACT_SHEET_MIDDLE.jpg`
- `GPT_OVERLAY_CONTACT_SHEET_LATE.jpg`

## Required review order

1. Validate engineering summary/cache/read-only gates from the bundle.
2. Compare per-result Pose Recovery and Evidence Quality fields.
3. Cross-check JSON against EARLY/MIDDLE/LATE contact sheets.
4. Decide PASS/FREEZE vs FAIL_NEEDS_SMALL_PATCH.
