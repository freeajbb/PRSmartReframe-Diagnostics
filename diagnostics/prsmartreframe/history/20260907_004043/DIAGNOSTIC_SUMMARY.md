# PRSmartReframe Diagnostic Summary

- Version: `0.4.92`
- Phase: `Phase 5B-4B Transaction / Rollback Negative Safety Matrix`
- Generated: `20260907_004043`
- Sanitized: `YES`
- Redactions: `109`
- Included files: `49`

## GPT analysis request

Please inspect this diagnostic directory as a whole. Start with `manifest.json`, then prefer the shallow `GPT_ANALYSIS_BUNDLE.json` and GPT contact-sheet bridge files. For Phase 5B-4B first verify source Reservation SHA, transactionId / fingerprint, Original Receipt path + SHA unchanged, Written Fixture post-state / component identity, B4B-01/02 no mutation RPC dispatch, B4B-03/04/05 exactly one rollback mutation RPC dispatch and Negative Premiere Writes 0, observationObserved/exclusive, Written Baseline Restore for B4B-03/04/05, 5/5 conservation, Fixture=2 / Negative=0 / Cleanup=1 / Total=3, Provider Calls=0, Final Cleanup uses the Original Receipt, and Original Before-State exact restore. Then inspect frozen Phase 5B-4A evidence for source reservation SHA, exact Baseline fingerprint/before-state authority, exactly one selected abnormality per Case, wouldWrite=false, exact Baseline Restore, 7-case conservation, Unexpected READY=0, Premiere Write Calls 0, Provider Calls 0, and Host Mutation=false. For frozen Phase 5B-3 evidence verify source reservation SHA, Fresh pre-write Host state, exact fingerprint/before-state gate, write/readback/ownership, measured Premiere Write Calls, Provider Calls 0, immutable transaction receipt, and Dedicated Rollback only if present. Then inspect Phase 5B-2 authorization/reservation authority and Phase 5B-1 READY/BLOCKED/STALE/INVALID/FAILED conservation, ExecutionReady, READY-only immutable plans, and JSON authority over imagery. Then for Phase 5A-2 verify only HUMAN_REVIEW entered Queue, review revisions are append-only, stale historical approvals are not current, executionReady/writeAllowed/applyAllowed=false, batch review OFF, and zero writes/providers. Then review Phase 5A-1 Candidate Queue before upstream phases. For Phase 4D-2 C4D2R-01, review the current `premiere_adapter_preview_batch.json`, all Adapter results, and the C4D2 contact sheets; verify current result conservation, Canonical Math only for eligible non-skipped results, required Round-trip, verified Motion and Geometry2 Host Contracts, Target Transform Ownership with Existing Geometry2 overwrite-forbidden, Frame-size Scaling Discovery authority/candidates, Scale-to-Frame UNKNOWN remains unknown; Frame Mapping prerequisite may use Verified Effective Mapping; Existing Geometry2 Ownership and final safety Gate remain frozen. premiereWriteCalls=0/providerCalls=0/Apply OFF. For upstream Phase 4D-1, verify current READY/SKIPPED/FAILED conservation, no fake geometry for SKIPPED, real 9:16 strategy geometry plus raw coverage/motion metrics for READY, QA requested/resolved conservation when present, premierePositionComputed=false, Apply OFF, Transform/Keyframe Write OFF and Premiere READ ONLY. Cross-check Phase 4C-7 Readiness and Phase 4C-6 Fusion when a Preview result is inconsistent.

## Current exported evidence

- Phase 5B-4B current evidence: Cases 0 / 5; PASS 0 / FAIL 0 / INCOMPLETE 5; Fixture Apply Writes 2; Negative Writes 0; Cleanup Writes 0; Total Controlled Writes 2; Unexpected Negative Writes 0; Provider Calls 0; Original Receipt SHA Unchanged true; Final Cleanup PENDING; Final Before-State Restore PENDING; Matrix Status PHASE5B4B_TRANSACTION_ROLLBACK_NEGATIVE_SAFETY_MATRIX_IN_PROGRESS.
- Phase 5B-3 current evidence: Input 1 / Result 1 = Write Verified 1 / BLOCKED 0 / STALE 0 / INVALID 0 / FAILED 0 / Auto Rollback Verified 0 / Auto Rollback Failed 0; Premiere Write Calls 2 / Provider Calls 0.
- Phase 5B-2 current evidence: Input 1 / Result 1 = AUTHORIZED 1 / BLOCKED 0 / STALE 0 / INVALID 0 / FAILED 0; Reservations 1; Premiere Write Calls 0 / Provider Calls 0; writeAllowed=false / applyAllowed=false. Authorization != Apply.
- Phase 5B-1 current evidence: Input 3 / Result 3 = READY 1 / BLOCKED 2 / STALE 0 / INVALID 0 / FAILED 0; ExecutionReady 1; Premiere Write Calls 0 / Provider Calls 0.
- Phase 5A-2 current evidence: Queue 3 = PENDING 2 / DECISION_RECORDED 1 / STALE 0 / SUPERSEDED 0 / INVALID 0; APPROVE 1 / REJECT 0 / REANALYZE 0 / DEFER 0; Premiere Write Calls 0 / Provider Calls 0.
- Phase 5A-1 current evidence: 3 results = AUTO_READY 0 / HUMAN_REVIEW 3 / SKIPPED 0 / FAILED 0; Human Review ordinals #01, #02, #03; Skipped ordinals none; Failed ordinals none; Reanalysis Required ordinals none.

## Privacy

This export was automatically sanitized. Session tokens, common API/access tokens, Authorization/Cookie values, passwords/secrets, and the Windows username segment in `C:\Users\...` paths are redacted before Git publication. No GitHub credential is stored in this diagnostic directory.
