# S.8: Incident Templates

> From: Vibe Coding Bible, Vol 1 — Appendix S
>
> Interactive skill version: [vibe-coding-starter](https://github.com/mnemoverse/vibe-coding-starter)

## S.8.1 Webhook Backlog Incident

**Symptom:** Backlog age exceeds threshold, events are not being processed.

**Fast checks:**
- Check worker health and error rate
- Check lease contention or lock issues
- Check provider API availability

**Containment:**
- Pause non-critical processing
- Increase worker capacity if safe
- Communicate delay to affected customers if needed

**Diagnosis / Fix / Verification** — see Appendix L for the Evidence-First methodology.

---

## S.8.2 Double Charge Complaint

**Symptom:** Customer reports being charged twice for the same period.

**Fast checks:**
- Locate all payment attempts for the customer
- Check idempotency keys and duplicates
- Check provider dashboard for actual charges

**Containment:**
- Acknowledge the complaint
- Do not issue refund until diagnosis is complete

---

## S.8.3 Missing Access Complaint

**Symptom:** Customer reports missing access despite payment.

**Fast checks:**
- Verify payment status in provider
- Check entitlement grant records
- Check decision records for the customer

**Containment:**
- Grant temporary access via override if payment is verified

---

## S.8.4 Suspected Account Takeover

**Stop the bleeding:** Revoke all sessions, disable sensitive actions temporarily, block high-velocity login attempts.

**Verify truth:** Audit timeline for login, recovery, passkey changes, role changes. Look for unfamiliar device and rapid action sequence.

**Restore safely:** Require recovery with stronger verification, add passkey, reset credentials, review memberships and roles.

---

## S.8.5 Lockout Storm

**Stop the bleeding:** Increase throttling, add temporary friction, protect recovery endpoints.

**Verify truth:** Measure volume by identifier and IP, confirm enumeration-safe errors.

**Restore safely:** Ensure real users can still recover, avoid attacker-driven permanent locks.

---

## S.8.6 Bulk Session Revocation After Leak

**Stop the bleeding:** Revoke all sessions, rotate secrets and tokens, invalidate refresh tokens.

**Verify truth:** Confirm which secrets leaked, where they were used, which accounts were impacted.

**Restore safely:** Deploy new secrets, reissue sessions, require re-auth, review audit for unusual activity during exposure window.

---

*For full context and when to use each prompt, see Appendix S in the Vibe Coding Bible.*
