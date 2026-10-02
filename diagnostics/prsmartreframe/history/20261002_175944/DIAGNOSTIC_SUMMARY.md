# PRSmartReframe Diagnostic Summary

- Version: `0.7.2.14`
- Phase: `Candidate · Task14C Stall Diagnostics + Pose Fail-Closed Hotfix V1`
- Generated: `20261002_175944`
- Sanitized: `YES`
- Redactions: `2706`
- Included files: `1003`

## GPT analysis request

Please inspect this diagnostic directory as a whole. Start with `manifest.json`, then prefer the shallow `GPT_ANALYSIS_BUNDLE.json`. When Phase 5B-6 evidence is present, review it first: Admission decision, current runtime state, immutable Admission integrity, execution-order/items digests, stale/invalid authority acceptance, current Preflight result, Admission/Preflight Premiere Writes, mutation dispatches, Provider Calls, and confirmation that Production Apply / Production Use / Batch Apply remain OFF. Phase 5B-6 generated summaries are diagnostic audit-only and never by themselves prove Windows Acceptance PASS. Then review Phase 5B-5 as the frozen upstream mutation baseline and explicitly answer: Duplicate Dispatch? Receipt-less COMMITTED? Unknown mutation followed by later execution? Parallel Host Mutation? Unverified item executed? Verify executionOrder, restart reconciliation, negative writes, provider calls, Receipt/Reservation/Ledger authority and Dedicated Rollback evidence. For Phase 5B-4B first verify source Reservation SHA, Original Receipt SHA, Written Fixture, mutation RPC behavior, Negative Premiere Writes, Written Baseline Restore, Final Cleanup, and Original Before-State. Continue through Phase 5B-4B / 5B-4A / 5B-3 / 5B-2 / 5B-1 and upstream preview phases as applicable.

## Current exported evidence

- API Middle-Frame Composition current evidence: RunId api05101_20261002_175807_843432; Apply Mode FAST_APPLY; Fast Apply Status FAST_APPLY_COMMITTED; Selected 109; Position Writes 102; No-op 7; Failures 0; Transactions 1; Rollback Available false; Records Written 0; Analysis Source WAITING_APPLY; Logical Requests 2; Provider Calls/Retries 2/0; Batch requested/effective 30/30; Concurrency requested/peak 3/2; Fast Apply runtime telemetry only; no rollback authority or durable Apply receipt.

## Privacy

This export was automatically sanitized. Session tokens, common API/access tokens, Authorization/Cookie values, passwords/secrets, and the Windows username segment in `C:\Users\...` paths are redacted before Git publication. No GitHub credential is stored in this diagnostic directory.
