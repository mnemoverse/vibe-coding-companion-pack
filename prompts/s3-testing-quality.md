# S.3: Testing & Quality

> From: Vibe Coding Bible, Vol 1 — Appendix S
>
> Interactive skill version: [vibe-coding-starter](https://github.com/mnemoverse/vibe-coding-starter)

## S.3.1 Unit Test Draft

**Prompt:**

> "Write unit tests for [FUNCTION/MODULE]. Cover happy path, one edge case, and one error case. Use [TESTING FRAMEWORK]."

**Tired version:**

> "Write one unit test for [FUNCTION]."

**Output:** A test file you can run immediately.

---

## S.3.2 Smoke Test Checklist

**Prompt:**

> "Create a post-deploy smoke test checklist for [APP NAME]. Include auth flow, core CRUD operations, and one integration point."

**Tired version:**

> "Write a 5-item smoke test checklist."

**Output:** A post-deploy verification checklist.

---

## S.3.3 Test Map (Must-Never-Break)

**Prompt:**

> "Given this app description, produce a test map with 12 must-never-break statements. Each statement should be testable and written from the user or system promise perspective. Output only the statements."

**Tired version:**

> "List 8 must-never-break behaviors for this app. Output only the list."

**Output:** A test map for `TEST-MAP.md` — the backbone of your test strategy.

---

## S.3.4 Intent-Based Test Rewrite

**Prompt:**

> "Convert this existing test into an intent-based test. Keep the public boundary, add at least one negative case, and ensure the assertions describe a promise, not an implementation detail. Output only the revised test."

**Tired version:**

> "Give me one intent test idea for this feature and the exact assertion it should make."

**Output:** A better test that survives refactoring.

---

## S.3.5 Integration Test Suite Design

**Prompt:**

> "Design an integration test suite for webhooks and background jobs for this app. Output exactly 6 tests with a short name and one-sentence intent for each. Include at least two negative tests. No code."

**Tired version:**

> "Give me 3 integration tests I must have for webhooks and jobs. Output only the names and intent."

**Output:** An integration test plan.

---

## S.3.6 Property-Based Test Idea

**Prompt:**

> "Propose one property-based test for [HANDLER]. Output the property in one sentence, the range of inputs to generate, and the single strongest invariant to assert. No code."

**Tired version:**

> "One property test idea for this handler. Output only the property and invariant."

**Output:** A property test idea that catches edge cases you would never write by hand.

---

## S.3.7 Flaky Test Diagnosis

**Prompt:**

> "This test is flaky. Diagnose likely sources of nondeterminism and propose three fixes. Output only: Cause, Fix, Verification step for each."

**Tired version:**

> "Give me 3 common causes of flakiness here and one fix for each."

**Output:** A diagnosis and fix plan for flaky tests.

---

## S.3.8 Payment Test Map

**Prompt:**

> "Create a test map for this payment integration. List 10 must-never-break behaviors covering: duplicates, out-of-order, renewals, refunds, and disputes. Output only the list."

**Tired version:**

> "List 6 payment tests we must have. Output only the list."

**Output:** A payment-specific test map.

---

## S.3.9 Auth Test Map

**Prompt:**

> "Create an auth test map with 25 tests grouped into unit, integration, browser reality, chaos. Each test must link to an invariant."

**Tired version:**

> "List 10 auth tests we must have. Output only the list."

**Output:** A comprehensive auth test strategy.

---

## S.3.10 Data Boundary Test Suite

**Prompt:**

> "Propose a minimal data test suite. Group by boundary: ingestion, raw_to_clean, truth_surface. For each test: what it prevents, how to compute it, and whether it should block publish or warn."

**Tired version:**

> "Pick the top 3 data tests for trust in a small SaaS and explain why in one sentence each."

**Output:** Data quality tests that protect trust.

---

## S.3.11 Metric Contract File

**Prompt:**

> "Convert this metric spec into a contract file. Output a simple YAML with fields: name, version, grain, time_semantics, required_fields, constraints, expected_ranges, publish_behavior. Keep checks high-value and maintainable."

**Tired version:**

> "Give me 5 contract checks for [METRIC NAME]. Mark each as block or warn."

**Output:** A runnable metric contract.

---

*For full context and when to use each prompt, see Appendix S in the Vibe Coding Bible.*
