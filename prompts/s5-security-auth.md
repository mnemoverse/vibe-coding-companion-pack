# S.5: Security & Auth

> From: Vibe Coding Bible, Vol 1 — Appendix S
>
> Interactive skill version: [vibe-coding-starter](https://github.com/mnemoverse/vibe-coding-starter)

## S.5.1 Threat Model (Top 10)

**Prompt:**

> Create a lightweight threat model for [APP NAME]. Output a table with 8 rows and 4 columns: Asset, Entry point, Threat, Minimum control. Keep controls small-team-friendly.

**Tired version:**

> List 6 realistic threats for this app and one control for each.

**Output:** A threat model table for `THREAT-MODEL.md`.

---

## S.5.2 OWASP Practical Checklist

**Prompt:**

> Map this app to a practical OWASP-style checklist. Output 10 bullets. Each bullet: risk category, what it means here, and one minimum control we can implement now.

**Tired version:**

> Give me 8 security checklist items aligned with common OWASP risks.

**Output:** A practical security checklist, not a theoretical framework.

---

## S.5.3 Secrets and Logging Policy

**Prompt:**

> Write a one-page secrets and logging policy. Include what must never be logged, redaction rules, how to store secrets safely, rotation schedule, and emergency revoke steps. Tool-agnostic.

**Tired version:**

> Write rules: what never to log and how to store secrets.

**Output:** A secrets policy for `SECRETS.md`.

---

## S.5.4 Session Handling Risk Review

**Prompt:**

> Review this sign-in and session approach. Output a list of 10 risks or mistakes that could lead to session confusion or bypass, and one mitigation for each. Keep it practical.

**Tired version:**

> List 6 session handling mistakes to avoid here.

**Output:** A session security review.

---

## S.5.5 Authorization Rules Extraction

**Prompt:**

> List all authorization rules implied by this set of endpoints. Output each rule as: Subject, Action, Object, Rule sentence. Keep it to 12 rules max.

**Tired version:**

> Write 6 authorization rules for this app in plain English.

**Output:** Explicit authorization rules you can implement and test.

---

## S.5.6 Dependency Verification

**Prompt:**

> I want to add this dependency suggested by an AI. Output a quick verification checklist with 10 checks max, including existence, maintainer signals, versioning, and alternative options.

**Tired version:**

> Give me a 6-step dependency verification checklist.

**Output:** A safety check before adding AI-suggested packages.

---

## S.5.7 Supply Chain Baseline

**Prompt:**

> Design a minimum supply chain baseline for this app. Output 10 steps max covering pinning, SBOM generation, vulnerability scanning, and an emergency update process.

**Tired version:**

> Give me 6 supply chain rules for a small team.

**Output:** A supply chain security baseline.

---

## S.5.8 Signature Verification Checklist

**Prompt:**

> Create a signature verification checklist for webhooks. Include: header extraction, timestamp validation, replay window, and key rotation handling. Output only the checklist.

**Tired version:**

> List 5 steps for webhook signature verification.

**Output:** A webhook security checklist.

---

## S.5.9 No Foot Guns Contract

**Prompt:**

> Write a No Foot Guns Contract for a multi-org app with [AUTH METHODS]. Output 12 testable invariants.

**Tired version:**

> List 8 auth invariants that must always be true.

**Output:** An auth contract that catches the dangerous defaults.

---

*For full context and when to use each prompt, see Appendix S in the Vibe Coding Bible.*
