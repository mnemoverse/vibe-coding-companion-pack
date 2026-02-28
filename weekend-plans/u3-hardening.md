# U.3: Hardening & Security

> From: Vibe Coding Bible, Vol 1 — Appendix U

*For: Adapted from Vol 1 (Ship-Ready Bar) and Vol 6 (Security Baseline).*

## 2h: Ship-Ready Bar Audit

1. Run the Ship-Ready Bar checklist against your project:
   - [ ] Auth protects every sensitive route
   - [ ] Inputs are validated server-side
   - [ ] Errors do not leak stack traces to users
   - [ ] Secrets are in environment variables, not code
   - [ ] Dependencies have no known critical vulnerabilities (`npm audit` / `pip audit`)
2. Identify the top 2 gaps
3. Fix one of them completely
4. Document the other as a TODO with a plan

**Done when:** You know your security posture and closed one gap.

**Tired version:** Just run the checklist and write down the gaps. Awareness is the first step.

## 6h: Close Gaps + Smoke Tests

1. Complete the 2h plan
2. Fix the second gap from your audit
3. Add rate limiting to your most sensitive endpoint (login, signup, or payment)
4. Write smoke tests that verify: auth works, invalid input is rejected, error pages render
5. Run `npm audit fix` or equivalent and verify nothing broke
6. Deploy to staging and run smoke tests there
7. Commit

**Done when:** Top 2 security gaps closed. Smoke tests verify the fixes. Staging is clean.

## 12h: Full Security Baseline + Deploy Rehearsal

1. Complete the 6h plan
2. Add CSRF protection if using forms
3. Add Content Security Policy headers
4. Review all API endpoints for authorization (not just authentication)
5. Add audit logging for sensitive actions (login, permission changes, data deletion)
6. Do a full deploy rehearsal: deploy to production, run smoke tests, verify alerts fire on simulated error
7. Write a one-page security runbook: what to do if you suspect a breach
8. Commit and tag

**Done when:** Full security baseline in place. Deploy rehearsal completed. Runbook written.

---

*For the philosophy behind time-boxed practice and the 2h/6h/12h format, see Appendix U in the Vibe Coding Bible.*
