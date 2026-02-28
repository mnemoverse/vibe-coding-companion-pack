# No Silent Failures Contract

> From: Vibe Coding Bible, Vol 1 — Appendix M

Applies to any background work: queues, scheduled jobs, automation, webhooks. The principle is simple: **every job must end in a visible outcome.**

## The Four Outcomes

Every background job must end in exactly one of:

| Outcome | Meaning | What Happens Next |
|---------|---------|-------------------|
| **Done** | Completed successfully with proof | Nothing — the system is healthy |
| **Failed** | Terminated with a recorded error | Appears in inbox, requires attention |
| **Needs Attention** | Cannot proceed without a human decision | Escalated to operator with context |
| **Not Needed** | Intentionally skipped or superseded | Recorded with reason, not silently dropped |

## The Contract

- "Retrying" is a transition, never a final state
- Stalled jobs become visible items, never invisible limbo
- Dead letters flow to an inbox, not a graveyard
- Every execution writes an attempt record
- Idempotency makes replay safe
- Reconciliation makes misses visible

## Trust Rules

1. **The UI never lies.** If it says "saved," the server confirmed it. If it says "sent," the job completed.
2. **The server owns truth.** Client-provided IDs are not trusted. Session context determines identity.
3. **Failures are visible.** No silent swallowing. No empty catch blocks. No logs that nobody reads.
4. **Idempotency is a requirement.** Any operation that can run twice will run twice. Design for it.
5. **Proof before merge.** Tests, reviews, and quality gates are blockers, not suggestions.

---

*For the ethics and legal dimensions, see Appendix E. For debugging when things go wrong, see Appendix L. For full context, see Appendix M in the Vibe Coding Bible.*
