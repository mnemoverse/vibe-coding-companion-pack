# U.4: Authentication Weekend

> From: Vibe Coding Bible, Vol 1 — Appendix U

*For: Adapted from Vol 8: Authentication Spine.*

## 2h: Data Model + One Login Method

1. Design the auth data model: users table, sessions table, password hashes
2. Implement one login method (email/password or OAuth)
3. Add session creation on successful login
4. Add a protected route that returns 401 without a valid session
5. Write one test: valid credentials return a session token

**Done when:** You can log in and access a protected resource. One test passes.

**Tired version:** Design the data model and write the migration. No code, just the schema. Good schemas prevent bad weekends later.

## 6h: RBAC + Audit Events + Recovery

1. Complete the 2h plan
2. Add roles to the user model (at minimum: user, admin)
3. Add a middleware that checks role before allowing access to admin routes
4. Log audit events: login success, login failure, role change
5. Implement password reset flow: request token, validate token, set new password
6. Write tests for: role-based access denied, audit event created, password reset works
7. Commit

**Done when:** RBAC works. Audit trail exists. Users can recover their accounts.

## 12h: Full Auth Spine with Tests + Runbooks

1. Complete the 6h plan
2. Add account lockout after N failed login attempts
3. Add session expiry and refresh token flow
4. Add a second login method (OAuth if you started with password, or vice versa)
5. Write integration tests for the full login-to-logout lifecycle
6. Write a runbook: how to unlock a user, how to revoke all sessions, how to rotate secrets
7. Deploy and verify auth works in production
8. Commit and tag

**Done when:** Auth spine is production-grade. Two login methods. Lockout, refresh, audit. Runbooks written.

---

*For the philosophy behind time-boxed practice and the 2h/6h/12h format, see Appendix U in the Vibe Coding Bible.*
