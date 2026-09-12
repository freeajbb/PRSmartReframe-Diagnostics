# PRSmartReframe Diagnostic Summary

- Version: `0.5.00`
- Phase: `Phase 5B-5 Multi-Clip Transactional Apply Pilot`
- Generated: `20260912_124510`
- Sanitized: `YES`
- Redactions: `412`
- Included files: `158`

## GPT analysis request

Please inspect this diagnostic directory as a whole. Start with `manifest.json`, then prefer the shallow `GPT_ANALYSIS_BUNDLE.json`. When Phase 5B-6 evidence is present, review it first: Admission decision, current runtime state, immutable Admission integrity, execution-order/items digests, stale/invalid authority acceptance, current Preflight result, Admission/Preflight Premiere Writes, mutation dispatches, Provider Calls, and confirmation that Production Apply / Production Use / Batch Apply remain OFF. Phase 5B-6 generated summaries are diagnostic audit-only and never by themselves prove Windows Acceptance PASS. Then review Phase 5B-5 as the frozen upstream mutation baseline and explicitly answer: Duplicate Dispatch? Receipt-less COMMITTED? Unknown mutation followed by later execution? Parallel Host Mutation? Unverified item executed? Verify executionOrder, restart reconciliation, negative writes, provider calls, Receipt/Reservation/Ledger authority and Dedicated Rollback evidence. For Phase 5B-4B first verify source Reservation SHA, Original Receipt SHA, Written Fixture, mutation RPC behavior, Negative Premiere Writes, Written Baseline Restore, Final Cleanup, and Original Before-State. Continue through Phase 5B-4B / 5B-4A / 5B-3 / 5B-2 / 5B-1 and upstream preview phases as applicable.

## Current exported evidence

- Middle Position Single-Clip Canary current evidence: Admission REJECTED; Apply State NO_APPLY; Apply Dispatches 0; Apply Writes 0; Apply Receipt MISSING; Rollback Available false; Rollback State NO_ROLLBACK; Rollback Dispatches 0; Rollback Writes 0; Rollback Receipt MISSING; Final State NOT_RESTORED; Batch Apply OFF; Production Use OFF; Parallel Host Mutation OFF.
- Middle Position Adapter V2 current evidence: 7 results = VERIFIED 2 / REVIEW 1 / BLOCKED 4 / FAILED 0; Premiere Writes 0; Provider Calls 0; Production Authority Consumption 0.
- Middle Position Reframe V2 current evidence: 7 results = ACCEPTABLE 2 / REVIEW 1 / BLOCKED 4 / FAILED 0; Premiere Writes 0; Provider Calls 0; Production Authority Consumption 0.
- Phase 4C-7 current evidence: 7 results = READY 3 / BLOCKED 4 / FAILED 0; blocked ordinals #02, #03, #06, #07.

## Privacy

This export was automatically sanitized. Session tokens, common API/access tokens, Authorization/Cookie values, passwords/secrets, and the Windows username segment in `C:\Users\...` paths are redacted before Git publication. No GitHub credential is stored in this diagnostic directory.
