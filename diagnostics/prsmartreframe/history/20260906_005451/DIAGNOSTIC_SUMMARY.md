# PRSmartReframe Diagnostic Summary

- Version: `0.4.80`
- Phase: `Phase 5B-1 Fresh Execution Preflight / Execution Eligibility Preview`
- Generated: `20260906_005451`
- Sanitized: `YES`
- Redactions: `39`
- Included files: `20`

## GPT analysis request

Please inspect this diagnostic directory as a whole. Start with `manifest.json`, then prefer the shallow `GPT_ANALYSIS_BUNDLE.json` and GPT contact-sheet bridge files. For Phase 5B-1 first verify READY/BLOCKED/STALE/INVALID/FAILED conservation, ExecutionReady, READY-only immutable plans, premiereWriteCalls=0/providerCalls=0, and JSON authority over imagery. Then for Phase 5A-2 verify only HUMAN_REVIEW entered Queue, review revisions are append-only, stale historical approvals are not current, executionReady/writeAllowed/applyAllowed=false, batch review OFF, and zero writes/providers. Then review Phase 5A-1 Candidate Queue before upstream phases. For Phase 4D-2 C4D2R-01, review the current `premiere_adapter_preview_batch.json`, all Adapter results, and the C4D2 contact sheets; verify current result conservation, Canonical Math only for eligible non-skipped results, required Round-trip, verified Motion and Geometry2 Host Contracts, Target Transform Ownership with Existing Geometry2 overwrite-forbidden, Frame-size Scaling Discovery authority/candidates, Scale-to-Frame UNKNOWN remains unknown; Frame Mapping prerequisite may use Verified Effective Mapping; Existing Geometry2 Ownership and final safety Gate remain frozen. premiereWriteCalls=0/providerCalls=0/Apply OFF. For upstream Phase 4D-1, verify current READY/SKIPPED/FAILED conservation, no fake geometry for SKIPPED, real 9:16 strategy geometry plus raw coverage/motion metrics for READY, QA requested/resolved conservation when present, premierePositionComputed=false, Apply OFF, Transform/Keyframe Write OFF and Premiere READ ONLY. Cross-check Phase 4C-7 Readiness and Phase 4C-6 Fusion when a Preview result is inconsistent.

## Current exported evidence

- Phase 5B-1 current evidence: Input 2 / Result 2 = READY 0 / BLOCKED 2 / STALE 0 / INVALID 0 / FAILED 0; ExecutionReady 0; Premiere Write Calls 0 / Provider Calls 0.
- Phase 5A-2 current evidence: Queue 2 = PENDING 0 / DECISION_RECORDED 2 / STALE 0 / SUPERSEDED 0 / INVALID 0; APPROVE 0 / REJECT 1 / REANALYZE 1 / DEFER 0; Premiere Write Calls 0 / Provider Calls 0.
- Phase 5A-1 current evidence: 2 results = AUTO_READY 0 / HUMAN_REVIEW 2 / SKIPPED 0 / FAILED 0; Human Review ordinals #01, #02; Skipped ordinals none; Failed ordinals none; Reanalysis Required ordinals none.

## Privacy

This export was automatically sanitized. Session tokens, common API/access tokens, Authorization/Cookie values, passwords/secrets, and the Windows username segment in `C:\Users\...` paths are redacted before Git publication. No GitHub credential is stored in this diagnostic directory.
