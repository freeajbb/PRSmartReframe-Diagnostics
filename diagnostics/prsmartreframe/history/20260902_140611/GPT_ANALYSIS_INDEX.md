# GPT Analysis Bridge

- App: `PRSmartReframe 0.4.16`
- Goal: avoid deep GitHub blob traversal/cache misses.
- Start with `manifest.json`, then read the single shallow `GPT_ANALYSIS_BUNDLE.json`.
- C4C4R-03B Association V2 Visual QA is diagnostic-only and must not drive Composition.

## Shallow analysis artifacts

- `GPT_ANALYSIS_BUNDLE.json` — sanitized runtime state + desktop log + available Pose/FastVision batch and result JSONs
- `GPT_C4C4R03B_ASSOCIATION_V2_CONTACT_SHEET.jpg` — C4C4R-03B Association V2 Visual QA contact sheet (Face-to-Person Tie-break V2, remaining ambiguity, duplicate ROI, Pose evidence, diagnostic score)

## Required review order

1. Validate FastVision engineering/cache/read-only gates from the bundle.
2. Review C4C4R-03B Association V2 Visual QA for Face-to-Person Tie-break V2 resolutions, remaining AMBIGUOUS cases and duplicate-person evidence.
3. Cross-check POSE_USABLE/POSE_WEAK and physicalPersonEvidenceScore labels against the rendered people/faces.
4. Decide whether Tie-break V2 safely reduces ambiguity without introducing wrong Face-to-Person matches; keep Composition and Apply OFF.
