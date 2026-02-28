# Ship-Ready Bar

> From: Vibe Coding Bible, Vol 1 — Appendix M

Comprehensive production readiness checklist. The goal is not perfection — the goal is to avoid the predictable failure modes that damage trust.

## Product Truth

- [ ] The UI never says "Saved" without server confirmation
- [ ] On failed save, user input remains visible and recoverable
- [ ] Error messages are calm, specific, and actionable
- [ ] Empty states guide the user toward the next action

## Ownership and Access

- [ ] Every record belongs to exactly one user (or org)
- [ ] Every read and write operation enforces ownership on the server side
- [ ] The server derives user identity from session context, not client-provided IDs
- [ ] Unauthorized access does not reveal whether a resource exists

## Validation

- [ ] Required fields are enforced on the server, not just the client
- [ ] Maximum lengths exist for all text inputs
- [ ] Input types are verified (no strings where numbers are expected)
- [ ] Normalization is applied consistently (casing, whitespace, duplicates)

## Auth and Credentials

- [ ] Passwords are stored only as strong hashes, never plaintext
- [ ] Reset tokens are one-time use and short-lived
- [ ] On password reset, existing sessions are invalidated
- [ ] Rate limiting exists for sign-in and reset requests

## Secrets and Logging

- [ ] No secrets are committed to the repo
- [ ] Logs never contain passwords, tokens, session IDs, reset links, or PII
- [ ] Structured logs include request IDs and event names
- [ ] Sensitive data is redacted by default

## Persistence and Migrations

- [ ] Schema changes go through migrations or tracked evolution
- [ ] Migrations are reviewed and tested before production
- [ ] A backup exists before risky deployments
- [ ] You have a restore procedure written down

## CI and Quality Gates

- [ ] Formatting and linting are automated and consistent
- [ ] Tests run in CI on every change that matters
- [ ] CI failures are treated as blockers, not suggestions
- [ ] One command exists to run all checks locally

## Deploy and Post-Deploy

- [ ] Deploy playbook exists and is followed
- [ ] Post-deploy smoke tests cover critical flows
- [ ] Monitoring signals exist for error rate and core failures
- [ ] Rollback plan exists and has been rehearsed at least once

---

If you can check most of these boxes, you are in a safe zone for an MVP. If you cannot, the fastest path is not adding features. It is closing the gap.

*For full context, see Appendix M in the Vibe Coding Bible.*
