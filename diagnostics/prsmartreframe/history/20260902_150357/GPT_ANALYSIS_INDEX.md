# GPT Analysis Bridge

- App: `PRSmartReframe 0.4.18`
- Goal: avoid deep GitHub blob traversal/cache misses.
- Start with `manifest.json`, then read the single shallow `GPT_ANALYSIS_BUNDLE.json`.
- C4C4R-04A Duplicate Group / Subject Count Uncertainty / Multi-person Ambiguity V3 Visual QA is diagnostic-only and must not drive Composition.
- C4C4R-03B Association V2 remains a frozen-candidate diagnostic reference.

## Shallow analysis artifacts

- `GPT_ANALYSIS_BUNDLE.json` — sanitized runtime state + desktop log + available Pose/FastVision batch and result JSONs
- `GPT_C4C4R04_DUPLICATE_GROUP_AMBIGUITY_V2_CONTACT_SHEET.jpg` — C4C4R-04A duplicate-group / subject-count range / Multi-person Ambiguity V3 contact sheet
- `GPT_C4C4R03B_ASSOCIATION_V2_CONTACT_SHEET.jpg` — C4C4R-03B Association V2 Visual QA contact sheet (Face-to-Person Tie-break V2, remaining ambiguity, duplicate ROI, Pose evidence, diagnostic score)

## Required review order

1. Validate FastVision engineering/cache/read-only gates from the bundle.
2. Review C4C4R-04A Visual QA for duplicate-group membership, collapse/conflict guards, subject-count lower/upper bounds, confidence and Multi-person Ambiguity V3.
3. Cross-check the frozen-candidate C4C4R-03B Face-to-Person Tie-break V2 behavior when relevant.
4. Confirm no grouping suppresses Frozen Person candidates and keep Composition and Apply OFF.
