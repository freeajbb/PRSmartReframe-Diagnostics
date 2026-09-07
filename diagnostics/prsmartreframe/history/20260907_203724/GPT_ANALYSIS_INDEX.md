# GPT Analysis Bridge

- App: `PRSmartReframe 0.4.99`
- Goal: avoid deep GitHub blob traversal/cache misses.
- Start with `manifest.json`, then read the single shallow `GPT_ANALYSIS_BUNDLE.json`.
- Phase 5B-5 has highest diagnostic priority when present. Treat its JSON/Receipt/Reservation/Ledger evidence as authority and generated summaries as audit-only. Explicitly answer: Duplicate Dispatch? Receipt-less COMMITTED? Unknown mutation followed by later execution? Parallel Host Mutation? Unverified item executed? Also verify executionOrder unchanged, restart reconciliation Premiere Writes=0 and mutation dispatches=0, Negative Premiere Writes=0, Provider Calls=0, and that Batch Apply / Production Apply / Production Use remain OFF.
- When Phase 5B-5 evidence is absent, Phase 5B-4B has highest diagnostic priority; otherwise Phase 5B-4B remains the frozen upstream verified baseline: verify source Reservation SHA, transactionId/fingerprint, Original Receipt SHA unchanged, Written Fixture post-state/component identity, B4B-01/02 mutation RPC not dispatched, B4B-03/04/05 exactly one rollback mutation RPC dispatched with Negative Premiere Writes=0, observationObserved/exclusive, Written Baseline Restore for B4B-03/04/05, 5/5 conservation, Fixture=2 / Negative=0 / Cleanup=1 / Total=3, Provider Calls=0, Final Cleanup using the original Receipt, and Original Before-State exact restore. Phase 5B-4A and Phase 5B-3 remain frozen upstream evidence.
- Phase 5B-1 remains the upstream eligibility authority: verify Input/READY/BLOCKED/STALE/INVALID/FAILED conservation, ExecutionReady, immutable READY-only execution plans, Premiere Write Calls 0, Provider Calls 0, and writeAllowed=false/applyAllowed=false before reviewing Phase 5A-2 and Phase 5A-1.
- Phase 5B-1 evidence rule: JSON = authority; Image = visual aid. Contact Sheet imagery cannot establish executionReady, SHA validity, or fingerprint validity.
- Phase 5A-2 reviews Human Review Queue + Review Decision Contract before Phase 5A-1: verify only HUMAN_REVIEW entered Queue, review revisions are append-only, stale historical approvals are not current, executionReady=false / writeAllowed=false / applyAllowed=false, batch review remains OFF, and zero writes/providers.
- Phase 5A-1 reviews Unified Eligibility / Candidate Queue: candidate_queue_batch.json is the batch authority; verify 1 input Clip -> 1 result conservation, AUTO_READY/HUMAN_REVIEW/SKIPPED/FAILED classification, Fresh/Stale/Broken chain behavior, and writeAllowed=false / premiereWriteCalls=0 / providerCalls=0. PHASE5A1_EXECUTION_GEOMETRY_AUTHORITY_V2 snapshots are audit-visible but diagnostics copies are never mutation-authority fallback.
- C4D2R-01 reviews Phase 4D-2 Premiere Adapter Preview: verify Snapshot / Canonical / Round-trip first; then Motion Host Contract, Source Geometry, Geometry2 Host Contract, Target Transform Ownership, Frame-size Scaling Discovery, Evidence Authority / Candidate list, Compatibility unchanged, and READ-ONLY safety. Existing Geometry2 must never be auto-overwritten; Scale-to-Frame UNKNOWN remains unknown; premiereWriteCalls=0.
- C4D1R-01 reviews Phase 4D-1 Composition Strategy / Position Preview: use the exported batch counts and ordinals as authority; READY clips must carry real 9:16 crop, coverage, motion and deterministic final quality; SKIPPED clips must have no fake geometry; premierePositionComputed=false and Premiere READ ONLY must remain visible.
- C4C7R-01 reviews Composition Readiness Hard Gate V1: every READY must satisfy every hard condition; every BLOCKED must carry deterministic machine-readable reasons from the exported batch; represented-person gaps and READ ONLY safety must remain visible.
- C4C6R-01 reviews Subject Fusion Preview V1: Frozen-ref integrity, semantic membership, Human Review propagation, primary decisions, fast-only modes, represented-person capability gaps, and PREVIEW-ONLY safety.
- C4C5R-03 reviews SlowVision Evidence V2: frame-scoped Frozen refs, semantic subject grouping, represented-person assessment, and deterministic human-review gating; it remains non-authoritative for Composition.
- C4C4R-03B Association V2 remains a frozen-candidate diagnostic reference.

## Current exported evidence

- Phase 5B-1 current evidence: Input 1 / Result 1 = READY 1 / BLOCKED 0 / STALE 0 / INVALID 0 / FAILED 0; ExecutionReady 1; Premiere Write Calls 0 / Provider Calls 0.
- Phase 5A-2 current evidence: Queue 1 = PENDING 0 / DECISION_RECORDED 1 / STALE 0 / SUPERSEDED 0 / INVALID 0; APPROVE 1 / REJECT 0 / REANALYZE 0 / DEFER 0; Premiere Write Calls 0 / Provider Calls 0.
- Phase 5A-1 current evidence: 1 results = AUTO_READY 0 / HUMAN_REVIEW 1 / SKIPPED 0 / FAILED 0; Human Review ordinals #01; Skipped ordinals none; Failed ordinals none; Reanalysis Required ordinals none.
- Phase 4D-2 current evidence: 1 results = READY 1 / REVIEW 0 / SKIPPED 0 / FAILED 0; Host Verified 1; skipped ordinals none.
- Phase 4D-1 current evidence: 1 results = READY 1 / SKIPPED 0 / FAILED 0; skipped ordinals none; Overview 1/1; READY Detail 3/3.
- Phase 4C-7 current evidence: 1 results = READY 1 / BLOCKED 0 / FAILED 0; blocked ordinals none.

## Shallow analysis artifacts

- `GPT_ANALYSIS_BUNDLE.json` — sanitized runtime state + desktop log + available Pose/FastVision/SlowVision batch and result JSONs
- `GPT_C4D2R01_PREMIERE_ADAPTER_OVERVIEW_CONTACT_SHEET.jpg` — C4D2R-01 full-batch Adapter Overview (READY/REVIEW/SKIPPED/FAILED + Canonical Math/Host status)
- `GPT_C4D2R01_PREMIERE_ADAPTER_DETAIL_CONTACT_SHEET.jpg` — C4D2R-01 Canonical Adapter detail (4D-1 frozen visual evidence → Virtual 1080x1920 target; NOT PREMIERE RENDER)
- `GPT_C4D1R01_COMPOSITION_PREVIEW_OVERVIEW_CONTACT_SHEET.jpg` — C4D1R-01 full-batch Overview (current READY/SKIPPED/FAILED propagation; SKIPPED has no fake crop)
- `GPT_C4D1R01_COMPOSITION_PREVIEW_READY_DETAIL_CONTACT_SHEET.jpg` — C4D1R-01 READY 3-frame detail (Frozen PRIMARY bbox + focus + desired/final 9:16 crop + coverage/motion quality)
- `GPT_C4C7R01_COMPOSITION_READINESS_CONTACT_SHEET.jpg` — C4C7R-01 Composition Readiness contact sheet (READY/BLOCKED + hard reasons + Frozen boxes; PREVIEW ONLY)
- `GPT_C4C6R01_SUBJECT_FUSION_CONTACT_SHEET.jpg` — C4C6R-01 Subject Fusion contact sheet (existing Frozen boxes only; fused/semantic labels + Human Review + primary decision)
- `GPT_C4C5R01_SLOW_VISION_EVIDENCE_CONTACT_SHEET.jpg` — C4C5R-03 SlowVision Evidence V2 quality contact sheet (legacy R01 filename retained for bridge compatibility; subject count + semantic grouping + represented person + deterministic review gate)
- `GPT_C4C4R05_SLOW_VISION_GATE_CONTACT_SHEET.jpg` — C4C4R-05 Slow-Vision escalation routing contact sheet (decision + reasons + count range + MPA)
- `GPT_C4C4R04_DUPLICATE_GROUP_AMBIGUITY_V2_CONTACT_SHEET.jpg` — C4C4R-04A duplicate-group / subject-count range / Multi-person Ambiguity V3 contact sheet
- `GPT_C4C4R03B_ASSOCIATION_V2_CONTACT_SHEET.jpg` — C4C4R-03B Association V2 Visual QA contact sheet (Face-to-Person Tie-break V2, remaining ambiguity, duplicate ROI, Pose evidence, diagnostic score)

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
