# GPT Analysis Bridge

- App: `PRSmartReframe 0.4.79`
- Goal: avoid deep GitHub blob traversal/cache misses.
- Start with `manifest.json`, then read the single shallow `GPT_ANALYSIS_BUNDLE.json`.
- Phase 5B-1 has highest diagnostic priority: verify Input/READY/BLOCKED/STALE/INVALID/FAILED conservation, ExecutionReady, immutable READY-only execution plans, Premiere Write Calls 0, Provider Calls 0, and writeAllowed=false/applyAllowed=false before reviewing Phase 5A-2 and Phase 5A-1.
- Phase 5B-1 evidence rule: JSON = authority; Image = visual aid. Contact Sheet imagery cannot establish executionReady, SHA validity, or fingerprint validity.
- Phase 5A-2 reviews Human Review Queue + Review Decision Contract before Phase 5A-1: verify only HUMAN_REVIEW entered Queue, review revisions are append-only, stale historical approvals are not current, executionReady=false / writeAllowed=false / applyAllowed=false, batch review remains OFF, and zero writes/providers.
- Phase 5A-1 reviews Unified Eligibility / Candidate Queue: candidate_queue_batch.json is the batch authority; verify 1 input Clip -> 1 result conservation, AUTO_READY/HUMAN_REVIEW/SKIPPED/FAILED classification, Fresh/Stale/Broken chain behavior, and writeAllowed=false / premiereWriteCalls=0 / providerCalls=0.
- C4D2R-01 reviews Phase 4D-2 Premiere Adapter Preview: verify Snapshot / Canonical / Round-trip first; then Motion Host Contract, Source Geometry, Geometry2 Host Contract, Target Transform Ownership, Frame-size Scaling Discovery, Evidence Authority / Candidate list, Compatibility unchanged, and READ-ONLY safety. Existing Geometry2 must never be auto-overwritten; Scale-to-Frame UNKNOWN remains unknown; premiereWriteCalls=0.
- C4D1R-01 reviews Phase 4D-1 Composition Strategy / Position Preview: use the exported batch counts and ordinals as authority; READY clips must carry real 9:16 crop, coverage, motion and deterministic final quality; SKIPPED clips must have no fake geometry; premierePositionComputed=false and Premiere READ ONLY must remain visible.
- C4C7R-01 reviews Composition Readiness Hard Gate V1: every READY must satisfy every hard condition; every BLOCKED must carry deterministic machine-readable reasons from the exported batch; represented-person gaps and READ ONLY safety must remain visible.
- C4C6R-01 reviews Subject Fusion Preview V1: Frozen-ref integrity, semantic membership, Human Review propagation, primary decisions, fast-only modes, represented-person capability gaps, and PREVIEW-ONLY safety.
- C4C5R-03 reviews SlowVision Evidence V2: frame-scoped Frozen refs, semantic subject grouping, represented-person assessment, and deterministic human-review gating; it remains non-authoritative for Composition.
- C4C4R-03B Association V2 remains a frozen-candidate diagnostic reference.

## Current exported evidence

- No Phase 5A-2 / 5A-1 batch is present. No Phase 4D-2 / 4D-1 / 4C-7 batch is present in this export; apply the generic review rules below without assuming historical sample counts.

## Shallow analysis artifacts

- `GPT_ANALYSIS_BUNDLE.json` — sanitized runtime state + desktop log + available Pose/FastVision/SlowVision batch and result JSONs

## Required review order

Before Phase 5A-1, when Phase 5A-2 is present inspect human_review_decision_batch.json and immutable review_decisions revisions: verify only HUMAN_REVIEW entered Queue, append-only revision continuity, stale historical approvals have no current effect, executionReady=false, writeAllowed=false, applyAllowed=false, batch review OFF, and zero writes/providers.
Before the numbered upstream deep-dive, when Phase 5A-1 is present inspect candidate_queue_batch.json as the product-layer authority: verify current result conservation, status/reason/action ordinals, AUTO_READY still requires Fresh Preflight, writeAllowed=false, executionReady=false, premiereWriteCalls=0, providerCalls=0, Apply OFF and Production Use OFF.
1. Review C4D2R-01 first in this exact order: Snapshot / Canonical / Round-trip → Motion Host Contract → Source Geometry → Geometry2 Host Contract → Target Transform Ownership → Frame-size Scaling Discovery → Evidence Authority / Candidate list → Compatibility unchanged → READ-ONLY safety. Verify result conservation against the current exported batch; only current non-skipped Adapter results may carry Canonical Math; Geometry2 mapping must come from verified signature calibration; Existing Geometry2 must remain overwrite-forbidden; premiereWriteCalls=0.
2. Review C4D1R-01 upstream context: verify current READY/SKIPPED/FAILED conservation and current skipped ordinals, no fake geometry for SKIPPED, raw coverage/motion metrics for READY, QA requested/resolved conservation when a QA manifest is present, premierePositionComputed=false and Premiere READ ONLY.
3. Verify only NEEDS_SLOW_VISION clips were submitted to Phase 4C-5.
4. Validate FastVision engineering/cache/read-only gates from the bundle.
5. Review C4C5R-03 SlowVision Evidence V2 for frame-scoped ID correctness, semanticSubjects grouping, represented-person assessment, Face↔Person resolutions, and HUMAN_REVIEW_GATE_V1 calibration.
6. Review C4C6R-01 Subject Fusion: lost Frozen refs must be zero; semantic membership must reference existing Frozen refs; Human Review must never be downgraded; primary decisions must not force a winner; FRAME_LOCAL_ONLY must not invent cross-frame identity; represented-person/capability gaps must propagate.
7. Review C4C7R-01 Composition Readiness: READY must satisfy every hard check; current BLOCKED ordinals and reasons must align with Fusion evidence; represented-person gaps must not be hidden.
8. Cross-check C4C4R-05/R04A/R03B when Fusion/SlowVision evidence conflicts with FastVision evidence.
9. Confirm Phase 4D-2/4D-1 Composition Preview, Composition Readiness, Subject Fusion, SlowVision evidence, Composition Apply remain PREVIEW-only/non-authoritative/OFF and Premiere remains READ ONLY.
