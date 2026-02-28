# S.1: Specification & Planning

> From: Vibe Coding Bible, Vol 1 — Appendix S
>
> Interactive skill version: [vibe-coding-starter](https://github.com/mnemoverse/vibe-coding-starter)

## S.1.1 One-Page Product Spec

**Prompt:**

> "Write a one-page product spec for [APP NAME]. Users can [LIST CORE ACTIONS]. Include core user stories, non-goals, domain definitions, and success criteria. Keep it tool-agnostic."

**Tired version:**

> "Write a one-page spec for [APP NAME] with user stories, non-goals, and success criteria."

**Output:** A one-page markdown spec you can commit as `SPEC.md`.

---

## S.1.2 Domain Rules & Truth Rules

**Prompt:**

> "Draft a plain-English domain document for [APP NAME]. Define [LIST ENTITIES] and their relationships. List 10 domain rules. Add a Truth Rules section explaining what counts as saved and how the UI should represent failure. Tool-agnostic."

**Tired version:**

> "Define [LIST ENTITIES] and 10 rules. Add Truth Rules for saving."

**Output:** A domain document you can commit as `DOMAIN.md`.

---

## S.1.3 Data Shape (Fields & Constraints)

**Prompt:**

> "Design a tool-agnostic data shape for [LIST ENTITIES]. For each, list fields, required vs optional, constraints, uniqueness rules, and top queries that need indexes."

**Tired version:**

> "Give me tables for [LIST ENTITIES] with constraints and uniqueness."

**Output:** A schema document for `DATA-SHAPE.md`.

---

## S.1.4 Edge Cases

**Prompt:**

> "List the top 10 edge cases for [FEATURE]. For each edge case, describe what could go wrong and what the expected behavior should be."

**Tired version:**

> "List 5 edge cases for [FEATURE]."

**Output:** An edge case list to review before implementation.

---

## S.1.5 PRD Lite (Story Map)

**Prompt:**

> "Write a PRD Lite for [APP NAME]. Include: one-page outcome, user stories mapped to features, non-goals, success signals, and a scope knife (what to cut first if time runs out)."

**Tired version:**

> "Write a one-paragraph outcome and 5 user stories for [APP NAME]."

**Output:** A lightweight PRD for `PRD-LITE.md`.

---

## S.1.6 Minimal API Slice

**Prompt:**

> "Design a minimal API slice for [APP NAME]. List endpoints with methods, auth requirements, request/response shapes, and error codes. Keep it to the smallest set that makes the MVP work."

**Tired version:**

> "List the 5 core API endpoints for [APP NAME] with methods and auth."

**Output:** An API spec for `API-SLICE.md`.

---

## S.1.7 UX Skeleton (States)

**Prompt:**

> "Write a UX skeleton for [APP NAME]. For each screen, list: user goal, states (loading, empty, error, success, edge), and one interaction that matters. Keep it to 5 screens max."

**Tired version:**

> "List 3 screens with states: loading, empty, error, success."

**Output:** A UX skeleton for `UX-SKELETON.md`.

---

## S.1.8 Money Contract

**Prompt:**

> "Write a money contract for this payment integration. Use 6 to 8 bullets. Each bullet ties a billing event to an entitlement outcome. Include rules for: payment success, payment failure, refund, dispute, and subscription cancellation. Output only the contract."

**Tired version:**

> "Write 5 billing rules for this app. Output only the rules."

**Output:** A money contract for `MONEY-CONTRACT.md`.

---

## S.1.9 Metric Spec

**Prompt:**

> "Draft a one-page metric spec for [METRIC NAME]. Output sections: Definition, Grain, Time Semantics, Input Events, Filters, Dedup Rules, Late Arrival Policy, Edge Cases, Breaking Changes, Receipt Requirements, Owner. Use plain language. One page."

**Tired version:**

> "Write a clear definition for [METRIC NAME]. Output: definition, grain, time semantics. Nothing else."

**Output:** A metric spec for data trust.

---

## S.1.10 Production Definition

**Prompt:**

> "Given this feature description, write a production definition for it as 8 acceptance statements that must be true in production. Keep them testable and specific."

**Tired version:**

> "Turn this feature into 5 must-be-true statements for production. No explanations."

**Output:** A production definition — the bridge between spec and code.

---

## S.1.11 Production Contract

**Prompt:**

> "Write a one-page production contract for this app. Use 6 to 10 plain language promises that map to technical behaviors. Output only the contract."

**Tired version:**

> "Give me 6 user promises for this app that imply engineering requirements. Output only the promises."

**Output:** A production contract for `PRODUCTION-CONTRACT.md`.

---

*For full context and when to use each prompt, see Appendix S in the Vibe Coding Bible.*
