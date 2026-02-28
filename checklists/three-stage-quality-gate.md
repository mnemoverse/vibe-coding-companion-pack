# Three-Stage Quality Gate

> From: Vibe Coding Bible, Vol 1 — Appendix M

Three checklists for three critical moments. Short enough to actually use under pressure.

## Before Merge

- [ ] Tests pass locally
- [ ] Linter passes with no warnings
- [ ] Types check (if applicable)
- [ ] No secrets in diff
- [ ] No console.log or debug statements
- [ ] Error messages are user-friendly
- [ ] Auth checked on server side
- [ ] Change is small enough to review in one sitting

## Before Deploy

- [ ] All CI checks pass
- [ ] Migration tested on staging (if applicable)
- [ ] Environment variables set in target environment
- [ ] Rollback plan documented
- [ ] Smoke test ready to run immediately after deploy
- [ ] On-call aware (if applicable)

## After Deploy

- [ ] Smoke test executed and passing
- [ ] Logs checked for new errors
- [ ] Key metrics stable (error rate, response time, success rate)
- [ ] User-facing critical path tested manually
- [ ] If anything is wrong, rollback immediately — do not debug in production

---

*For the comprehensive production readiness checklist, see the Ship-Ready Bar. For full context, see Appendix M in the Vibe Coding Bible.*
