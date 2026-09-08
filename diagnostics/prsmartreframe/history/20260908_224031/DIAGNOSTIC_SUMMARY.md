# PRSmartReframe Diagnostic Summary

- Version: `0.5.00`
- Phase: `Phase 5B-5 Multi-Clip Transactional Apply Pilot`
- Generated: `20260908_224031`
- Sanitized: `YES`
- Redactions: `76`
- Included files: `29`

## GPT analysis request

Please inspect this diagnostic directory as a whole. Start with `manifest.json`, then prefer the shallow `GPT_ANALYSIS_BUNDLE.json`. When Phase 5B-6 evidence is present, review it first: Admission decision, current runtime state, immutable Admission integrity, execution-order/items digests, stale/invalid authority acceptance, current Preflight result, Admission/Preflight Premiere Writes, mutation dispatches, Provider Calls, and confirmation that Production Apply / Production Use / Batch Apply remain OFF. Phase 5B-6 generated summaries are diagnostic audit-only and never by themselves prove Windows Acceptance PASS. Then review Phase 5B-5 as the frozen upstream mutation baseline and explicitly answer: Duplicate Dispatch? Receipt-less COMMITTED? Unknown mutation followed by later execution? Parallel Host Mutation? Unverified item executed? Verify executionOrder, restart reconciliation, negative writes, provider calls, Receipt/Reservation/Ledger authority and Dedicated Rollback evidence. For Phase 5B-4B first verify source Reservation SHA, Original Receipt SHA, Written Fixture, mutation RPC behavior, Negative Premiere Writes, Written Baseline Restore, Final Cleanup, and Original Before-State. Continue through Phase 5B-4B / 5B-4A / 5B-3 / 5B-2 / 5B-1 and upstream preview phases as applicable.

## Current exported evidence

- Phase 5B-2 current evidence: Input 1 / Result 1 = AUTHORIZED 1 / BLOCKED 0 / STALE 0 / INVALID 0 / FAILED 0; Reservations 1; Premiere Write Calls 0 / Provider Calls 0; writeAllowed=false / applyAllowed=false. Authorization != Apply.
- Phase 5B-1 current evidence: Input 1 / Result 1 = READY 1 / BLOCKED 0 / STALE 0 / INVALID 0 / FAILED 0; ExecutionReady 1; Premiere Write Calls 0 / Provider Calls 0.
- Phase 5A-2 current evidence: Queue 1 = PENDING 0 / DECISION_RECORDED 1 / STALE 0 / SUPERSEDED 0 / INVALID 0; APPROVE 1 / REJECT 0 / REANALYZE 0 / DEFER 0; Premiere Write Calls 0 / Provider Calls 0.
- Phase 5A-1 current evidence: 1 results = AUTO_READY 0 / HUMAN_REVIEW 1 / SKIPPED 0 / FAILED 0; Human Review ordinals #01; Skipped ordinals none; Failed ordinals none; Reanalysis Required ordinals none.

## Privacy

This export was automatically sanitized. Session tokens, common API/access tokens, Authorization/Cookie values, passwords/secrets, and the Windows username segment in `C:\Users\...` paths are redacted before Git publication. No GitHub credential is stored in this diagnostic directory.
