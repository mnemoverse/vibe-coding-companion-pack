# Pre-Deployment Checklist

> From: Vibe Coding Bible, Vol 1 — Appendix M

Before any deployment:

## Security

- [ ] Ran `npm audit` (or equivalent) — no high/critical issues
- [ ] No hardcoded secrets (search for key, secret, password, token)
- [ ] Environment variables used for configuration
- [ ] HTTPS enforced
- [ ] Auth/authz working correctly

## Quality

- [ ] All tests passing
- [ ] No console.log/print statements in production code
- [ ] Error handling doesn't expose internals
- [ ] No commented-out code

## Operations

- [ ] Logging is appropriate (not too much, not too little)
- [ ] Health check endpoint works
- [ ] Deployment can be rolled back
- [ ] Monitoring is in place

---

*For the comprehensive production readiness checklist, see the Ship-Ready Bar. For context and code examples, see Appendix M in the Vibe Coding Bible.*
