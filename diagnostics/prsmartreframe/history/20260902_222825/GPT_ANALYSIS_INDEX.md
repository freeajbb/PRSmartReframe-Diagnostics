# GPT Analysis Bridge

- App: `PRSmartReframe 0.4.29`
- Goal: avoid deep GitHub blob traversal/cache misses.
- Start with `manifest.json`, then read the single shallow `GPT_ANALYSIS_BUNDLE.json`.
- C4C7R-01 reviews Composition Readiness Hard Gate V1: every READY must satisfy every hard condition; every BLOCKED must carry deterministic machine-readable reasons; known blocked cases #03/#05/#07/#13/#14/#15 must remain blocked; represented-person gaps and READ ONLY safety must remain visible.
- C4C6R-01 reviews Subject Fusion Preview V1: Frozen-ref integrity, semantic membership, Human Review propagation, primary decisions, fast-only modes, represented-person capability gaps, and PREVIEW-ONLY safety.
- C4C5R-03 reviews SlowVision Evidence V2: frame-scoped Frozen refs, semantic subject grouping, represented-person assessment, and deterministic human-review gating; it remains non-authoritative for Composition.
- C4C4R-03B Association V2 remains a frozen-candidate diagnostic reference.

## Shallow analysis artifacts

- `GPT_ANALYSIS_BUNDLE.json` — sanitized runtime state + desktop log + available Pose/FastVision/SlowVision batch and result JSONs
- `GPT_C4C7R01_COMPOSITION_READINESS_CONTACT_SHEET.jpg` — C4C7R-01 Composition Readiness contact sheet (READY/BLOCKED + hard reasons + Frozen boxes; PREVIEW ONLY)

## Required review order

1. Validate FastVision engineering/cache/read-only gates from the bundle.
2. Verify only NEEDS_SLOW_VISION clips were submitted to Phase 4C-5.
3. Review C4C5R-03 SlowVision Evidence V2 for frame-scoped ID correctness, semanticSubjects grouping, represented-person assessment, Face↔Person resolutions, and HUMAN_REVIEW_GATE_V1 calibration.
4. Review C4C6R-01 Subject Fusion: lost Frozen refs must be zero; semantic membership must reference existing Frozen refs; Human Review must never be downgraded; primary decisions must not force a winner; FRAME_LOCAL_ONLY must not invent cross-frame identity; represented-person/capability gaps must propagate.
5. Review C4C7R-01 Composition Readiness: READY must satisfy every hard check; BLOCKED reasons must align with Fusion evidence; #03/#05/#07/#13/#14/#15 must remain BLOCKED; represented-person gaps must not be hidden.
6. Cross-check C4C4R-05/R04A/R03B when Fusion/SlowVision evidence conflicts with FastVision evidence.
7. Confirm Composition Readiness, Subject Fusion, SlowVision evidence, Composition and Apply remain PREVIEW-only/non-authoritative/OFF and Premiere remains READ ONLY.
