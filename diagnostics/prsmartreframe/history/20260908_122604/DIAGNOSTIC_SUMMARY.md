# PRSmartReframe Diagnostic Summary

- Version: `0.5.01`
- Phase: `Phase 5B-6 Production Admission Safety Gate`
- Generated: `20260908_122604`
- Sanitized: `YES`
- Redactions: `24`
- Included files: `22`

## GPT analysis request

Please inspect this diagnostic directory as a whole. Start with `manifest.json`, then prefer the shallow `GPT_ANALYSIS_BUNDLE.json`. When Phase 5B-6 evidence is present, review it first: Admission decision, current runtime state, immutable Admission integrity, execution-order/items digests, stale/invalid authority acceptance, current Preflight result, Admission/Preflight Premiere Writes, mutation dispatches, Provider Calls, and confirmation that Production Apply / Production Use / Batch Apply remain OFF. Phase 5B-6 generated summaries are diagnostic audit-only and never by themselves prove Windows Acceptance PASS. Then review Phase 5B-5 as the frozen upstream mutation baseline and explicitly answer: Duplicate Dispatch? Receipt-less COMMITTED? Unknown mutation followed by later execution? Parallel Host Mutation? Unverified item executed? Verify executionOrder, restart reconciliation, negative writes, provider calls, Receipt/Reservation/Ledger authority and Dedicated Rollback evidence. For Phase 5B-4B first verify source Reservation SHA, Original Receipt SHA, Written Fixture, mutation RPC behavior, Negative Premiere Writes, Written Baseline Restore, Final Cleanup, and Original Before-State. Continue through Phase 5B-4B / 5B-4A / 5B-3 / 5B-2 / 5B-1 and upstream preview phases as applicable.

## Current exported evidence

- Phase 5B-6 current diagnostic evidence: Admission ADMITTED; Runtime ADMITTED; Integrity FAIL; Items 3; Latest Preflight EXECUTION_READY; Admission Writes 0; Mutation Dispatches 0; Provider Calls 0; Production Apply remains OFF. This is diagnostic audit evidence only; it does not by itself mark Phase 5B-6 Windows Acceptance PASS.
- Phase 5B-2 current evidence: Input 1 / Result 1 = AUTHORIZED 1 / BLOCKED 0 / STALE 0 / INVALID 0 / FAILED 0; Reservations 1; Premiere Write Calls 0 / Provider Calls 0; writeAllowed=false / applyAllowed=false. Authorization != Apply.
- Phase 5B-1 current evidence: Input 1 / Result 1 = READY 1 / BLOCKED 0 / STALE 0 / INVALID 0 / FAILED 0; ExecutionReady 1; Premiere Write Calls 0 / Provider Calls 0.

## Privacy

This export was automatically sanitized. Session tokens, common API/access tokens, Authorization/Cookie values, passwords/secrets, and the Windows username segment in `C:\Users\...` paths are redacted before Git publication. No GitHub credential is stored in this diagnostic directory.
