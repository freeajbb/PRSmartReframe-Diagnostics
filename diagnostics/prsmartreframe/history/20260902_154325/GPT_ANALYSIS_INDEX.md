# GPT Analysis Bridge

- App: `PRSmartReframe 0.4.19`
- Goal: avoid deep GitHub blob traversal/cache misses.
- Start with `manifest.json`, then read the single shallow `GPT_ANALYSIS_BUNDLE.json`.
- C4C4R-05 FastVision Confidence / Slow-Vision Escalation Gate Visual QA is routing-only and must not drive Composition.
- C4C4R-03B Association V2 remains a frozen-candidate diagnostic reference.

## Shallow analysis artifacts

- `GPT_ANALYSIS_BUNDLE.json` — sanitized runtime state + desktop log + available Pose/FastVision batch and result JSONs
- `GPT_C4C4R05_SLOW_VISION_GATE_CONTACT_SHEET.jpg` — C4C4R-05 Slow-Vision escalation routing contact sheet (decision + reasons + count range + MPA)
- `GPT_C4C4R04_DUPLICATE_GROUP_AMBIGUITY_V2_CONTACT_SHEET.jpg` — C4C4R-04A duplicate-group / subject-count range / Multi-person Ambiguity V3 contact sheet
- `GPT_C4C4R03B_ASSOCIATION_V2_CONTACT_SHEET.jpg` — C4C4R-03B Association V2 Visual QA contact sheet (Face-to-Person Tie-break V2, remaining ambiguity, duplicate ROI, Pose evidence, diagnostic score)

## Required review order

1. Validate FastVision engineering/cache/read-only gates from the bundle.
2. Review C4C4R-05 Visual QA for FAST_VISION_CONFIDENT vs NEEDS_SLOW_VISION and trigger reasons.
3. Use C4C4R-04A as the subject-count / duplicate-group evidence reference.
4. Cross-check C4C4R-03B Face-to-Person Tie-break V2 when relevant.
5. Confirm Slow Vision execution, Composition and Apply remain OFF.
