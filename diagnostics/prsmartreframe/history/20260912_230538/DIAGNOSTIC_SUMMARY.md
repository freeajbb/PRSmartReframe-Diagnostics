# PRSmartReframe Diagnostic Summary

- Version: `0.5.00`
- Phase: `Phase 5B-5 Multi-Clip Transactional Apply Pilot`
- Generated: `20260912_230538`
- Sanitized: `YES`
- Redactions: `54`
- Included files: `36`

## GPT analysis request

Please inspect this diagnostic directory as a whole. Start with `manifest.json`, then prefer the shallow `GPT_ANALYSIS_BUNDLE.json`. When Phase 5B-6 evidence is present, review it first: Admission decision, current runtime state, immutable Admission integrity, execution-order/items digests, stale/invalid authority acceptance, current Preflight result, Admission/Preflight Premiere Writes, mutation dispatches, Provider Calls, and confirmation that Production Apply / Production Use / Batch Apply remain OFF. Phase 5B-6 generated summaries are diagnostic audit-only and never by themselves prove Windows Acceptance PASS. Then review Phase 5B-5 as the frozen upstream mutation baseline and explicitly answer: Duplicate Dispatch? Receipt-less COMMITTED? Unknown mutation followed by later execution? Parallel Host Mutation? Unverified item executed? Verify executionOrder, restart reconciliation, negative writes, provider calls, Receipt/Reservation/Ledger authority and Dedicated Rollback evidence. For Phase 5B-4B first verify source Reservation SHA, Original Receipt SHA, Written Fixture, mutation RPC behavior, Negative Premiere Writes, Written Baseline Restore, Final Cleanup, and Original Before-State. Continue through Phase 5B-4B / 5B-4A / 5B-3 / 5B-2 / 5B-1 and upstream preview phases as applicable.

## Current exported evidence

- API Middle-Frame Composition current evidence: RunId api0565_20260912_225451_288188; ApplyBatchId api0565_apply_20260912_225536_463430; Analysis WAITING_APPLY; Logical Requests 1; Provider Calls/Retries 1/0; Batch requested/effective 10/10; Concurrency requested/peak 4/1; Apply Dispatches/Writes 1/1; Rollback Dispatches/Writes 1/1; Hard Stop false; Hard Stop Reason NONE; Production Use OFF; Parallel Host Mutation OFF; Automatic Resume OFF; Authority DIAGNOSTIC_AUDIT_ONLY.

## Privacy

This export was automatically sanitized. Session tokens, common API/access tokens, Authorization/Cookie values, passwords/secrets, and the Windows username segment in `C:\Users\...` paths are redacted before Git publication. No GitHub credential is stored in this diagnostic directory.
