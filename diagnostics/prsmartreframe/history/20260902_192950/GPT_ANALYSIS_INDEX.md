# GPT Analysis Bridge

- App: `PRSmartReframe 0.4.25`
- Goal: avoid deep GitHub blob traversal/cache misses.
- Start with `manifest.json`, then read the single shallow `GPT_ANALYSIS_BUNDLE.json`.
- C4C5R-03 reviews SlowVision Evidence V2: frame-scoped Frozen refs, semantic subject grouping, represented-person assessment, and deterministic human-review gating; it remains non-authoritative for Composition.
- C4C4R-03B Association V2 remains a frozen-candidate diagnostic reference.

## Shallow analysis artifacts

- `GPT_ANALYSIS_BUNDLE.json` — sanitized runtime state + desktop log + available Pose/FastVision/SlowVision batch and result JSONs
- `GPT_C4C5R01_SLOW_VISION_EVIDENCE_CONTACT_SHEET.jpg` — C4C5R-03 SlowVision Evidence V2 quality contact sheet (legacy R01 filename retained for bridge compatibility; subject count + semantic grouping + represented person + deterministic review gate)
- `GPT_C4C4R05_SLOW_VISION_GATE_CONTACT_SHEET.jpg` — C4C4R-05 Slow-Vision escalation routing contact sheet (decision + reasons + count range + MPA)
- `GPT_C4C4R04_DUPLICATE_GROUP_AMBIGUITY_V2_CONTACT_SHEET.jpg` — C4C4R-04A duplicate-group / subject-count range / Multi-person Ambiguity V3 contact sheet
- `GPT_C4C4R03B_ASSOCIATION_V2_CONTACT_SHEET.jpg` — C4C4R-03B Association V2 Visual QA contact sheet (Face-to-Person Tie-break V2, remaining ambiguity, duplicate ROI, Pose evidence, diagnostic score)

## Required review order

1. Validate FastVision engineering/cache/read-only gates from the bundle.
2. Verify only NEEDS_SLOW_VISION clips were submitted to Phase 4C-5.
3. Review C4C5R-03 SlowVision Evidence V2 for frame-scoped ID correctness, semanticSubjects grouping, represented-person assessment, Face↔Person resolutions, and HUMAN_REVIEW_GATE_V1 calibration.
4. Cross-check C4C4R-05/R04A/R03B when SlowVision evidence conflicts with FastVision evidence.
5. Confirm SlowVision evidence, Composition and Apply remain non-authoritative/OFF.
