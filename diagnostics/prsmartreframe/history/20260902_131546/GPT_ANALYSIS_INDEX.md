# GPT Analysis Bridge

- App: `PRSmartReframe 0.4.14`
- Goal: avoid deep GitHub blob traversal/cache misses.
- Start with `manifest.json`, then read the single shallow `GPT_ANALYSIS_BUNDLE.json`.
- C4C4R-03A Association Visual QA is diagnostic-only and must not drive Composition.

## Shallow analysis artifacts

- `GPT_ANALYSIS_BUNDLE.json` — sanitized runtime state + desktop log + available Pose/FastVision batch and result JSONs
- `GPT_C4C4R03A_ASSOCIATION_CONTACT_SHEET.jpg` — C4C4R-03A Association Visual QA contact sheet (Face-to-Person, duplicate ROI, Pose evidence, diagnostic score)

## Required review order

1. Validate FastVision engineering/cache/read-only gates from the bundle.
2. Review C4C4R-03A Association Visual QA for Face-to-Person MATCHED/AMBIGUOUS behavior and duplicate-person evidence.
3. Cross-check POSE_USABLE/POSE_WEAK and physicalPersonEvidenceScore labels against the rendered people/faces.
4. Decide whether Association v1 is visually acceptable or needs a small tie-break refinement; keep Composition and Apply OFF.
