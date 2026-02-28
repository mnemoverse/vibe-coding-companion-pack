# S.2: Building & Feature Implementation

> From: Vibe Coding Bible, Vol 1 — Appendix S
>
> Interactive skill version: [vibe-coding-starter](https://github.com/mnemoverse/vibe-coding-starter)

## S.2.1 Save Contract (UI States)

**Prompt:**

> "Design a tool-agnostic save contract for create and edit flows in [APP NAME]. Include UI states (idle, saving, saved, error), server validations, and rules that prevent the UI from claiming success before confirmation."

**Tired version:**

> "Write a save contract with states: saving, saved, error. Truth-first."

**Output:** A save contract that prevents premature success messages.

---

## S.2.2 Auth Pattern Decision Note

**Prompt:**

> "Compare session-based auth, token-based auth, and passwordless for [APP TYPE]. Recommend one for an MVP with a safe production path. Provide a decision record I can paste into docs."

**Tired version:**

> "Recommend an auth pattern for [APP TYPE] and write the decision note."

**Output:** An ADR (Architecture Decision Record) for auth.

---

## S.2.3 Protected Routes Plan

**Prompt:**

> "Write a protected routes plan for a multi-user app. Identify public vs protected routes, how to centralize checks, how to handle redirects, and how to avoid leaking whether a resource exists to unauthorized users."

**Tired version:**

> "List public vs protected routes and how to centralize auth checks."

**Output:** A routes security plan.

---

## S.2.4 Integration Map

**Prompt:**

> "Create an integration map for [APP NAME]. List all external systems, objects exchanged, who owns each, direction of data flow, and the failure surface for each integration. Output as a table."

**Tired version:**

> "List external systems, what we exchange, and one failure risk each."

**Output:** An integration map for `INTEGRATION-MAP.md`.

---

## S.2.5 Webhook Endpoint Scaffold

**Prompt:**

> "Design a webhook receiver for [PROVIDER]. Output: signature verification steps, persist-before-ack rule, response codes, retry expectations, and inbox table schema. Keep it tool-agnostic."

**Tired version:**

> "Write the 5 rules for a safe webhook receiver. Output only the rules."

**Output:** A webhook receiver spec.

---

## S.2.6 Idempotent Handler

**Prompt:**

> "Write pseudocode for an idempotent event handler with effect records. Handle: exact duplicates, retriable failures, and poison messages. Include idempotency key strategy. Output only the pseudocode."

**Tired version:**

> "Write 3 rules for idempotent event handling. Output only the rules."

**Output:** An idempotency pattern you can adapt to any queue/webhook system.

---

## S.2.7 Outbound Call Wrapper

**Prompt:**

> "Design a shared outbound call wrapper with timeouts, retries, exponential backoff with jitter, circuit breaker per provider, and rate limiting. Output the configuration parameters and their default values. Tool-agnostic."

**Tired version:**

> "List the 5 settings every outbound call wrapper needs. Output only the settings."

**Output:** A call wrapper spec for external API integrations.

---

## S.2.8 Four Outcomes Job Mapping

**Prompt:**

> "Create a Four Outcomes mapping table for [JOB TYPES]. Each job type must end in exactly one of: Done, Failed, Needs Attention, Not Needed. For each outcome, define what proof looks like. Output only the table."

**Tired version:**

> "Map [JOB TYPE] to four outcomes with one proof artifact each."

**Output:** A job outcomes contract for automation work.

---

## S.2.9 Session Lifecycle Spec

**Prompt:**

> "Write a session lifecycle spec: expiry, idle timeout, rotation triggers, revocation rules, and device list fields."

**Tired version:**

> "List 6 session rules: expiry, rotation, revocation. Output only the rules."

**Output:** A session spec that prevents auth foot-guns.

---

## S.2.10 RBAC Model

**Prompt:**

> "Propose an RBAC model with 3 to 5 roles and a permission vocabulary based on actions on resources."

**Tired version:**

> "List 3 roles and 8 permissions. Output only the model."

**Output:** A role-based access control model.

---

## S.2.11 Entitlement Mapping

**Prompt:**

> "Create an entitlement mapping for this SaaS. Input: provider plan ids. Output: internal feature flags. Include: active, trial, grace period, and revoked states. Output only the mapping."

**Tired version:**

> "Map 3 plan tiers to feature flags with 4 states."

**Output:** An entitlement mapping for payment integrations.

---

*For full context and when to use each prompt, see Appendix S in the Vibe Coding Bible.*
