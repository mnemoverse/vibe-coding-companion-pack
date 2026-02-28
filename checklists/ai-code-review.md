# AI Code Review Checklist

> From: Vibe Coding Bible, Vol 1 — Appendix M

Use this checklist before merging any AI-generated code.

## 1. Input Validation

- [ ] User inputs are validated before use
- [ ] Input lengths are bounded
- [ ] Input types are verified
- [ ] Dangerous characters are escaped or rejected

## 2. Authentication & Authorization

- [ ] Authentication is required where needed
- [ ] Authorization checks exist for protected resources
- [ ] Tokens/sessions have expiration
- [ ] Failed auth is logged appropriately

## 3. Sensitive Data

- [ ] Passwords are hashed (bcrypt, argon2), never stored plain
- [ ] Secrets are not hardcoded
- [ ] Sensitive data is not logged
- [ ] Sensitive data is encrypted at rest and in transit

## 4. Error Handling

- [ ] Errors don't expose internal details to users
- [ ] Stack traces are not shown in production
- [ ] Errors are logged with context for debugging
- [ ] Failed operations don't leave system in bad state

## 5. Dependencies

- [ ] No unnecessary dependencies added
- [ ] Dependencies are from trusted sources
- [ ] Dependencies are reasonably current
- [ ] No known vulnerabilities in dependencies

## 6. Code Quality

- [ ] No commented-out code
- [ ] No TODO/FIXME for critical items
- [ ] No obvious logic errors
- [ ] No infinite loops or unbounded recursion

---

*For code examples, red flags, and common vulnerability patterns, see Appendix M in the Vibe Coding Bible.*
