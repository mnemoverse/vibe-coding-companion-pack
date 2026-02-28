# S.7: Review & Refactoring

> From: Vibe Coding Bible, Vol 1 — Appendix S
>
> Interactive skill version: [vibe-coding-starter](https://github.com/mnemoverse/vibe-coding-starter)

## S.7.1 Code Review

**Prompt:**

> Review this code for security issues, error handling, and readability. List concerns in priority order. Be specific about line numbers.

**Tired version:**

> Review this code. List top 3 issues.

**Output:** A prioritized review with specific locations.

---

## S.7.2 Diff Summary

**Prompt:**

> Summarize this diff in one paragraph. Highlight any changes to auth, data access, or error handling.

**Tired version:**

> Summarize this diff.

**Output:** A PR description you can paste directly.

---

## S.7.3 Junior PR Review Checklist

**Prompt:**

> Review this change as if it were a junior developer PR. Produce a checklist of 12 review questions focused on security, correctness, and edge cases. Output only the checklist.

**Tired version:**

> Give me 6 security review questions for this endpoint.

**Output:** A review checklist that catches what humans miss when tired.

---

## S.7.4 Quality Rails Table

**Prompt:**

> Design a minimal quality rails checklist for this project. Output a table with three columns: Rail, Why it exists, How it is enforced. Keep it to 8 rails max.

**Tired version:**

> Give me 6 quality rails for this project.

**Output:** A quality rails summary for your README.

---

## S.7.5 Merge Gate Proposal

**Prompt:**

> Propose a minimal merge gate for this project with 6 checks max. Output each check with: purpose, command, and what to do when it fails.

**Tired version:**

> List the 4 checks my merge gate should require.

**Output:** A CI merge gate definition.

---

## S.7.6 Release Checklist

**Prompt:**

> Create a release checklist for this app. Output a numbered list of 12 steps max, including smoke tests and rollback steps. Keep it tool-agnostic and actionable.

**Tired version:**

> Give me a 6-step release checklist including rollback.

**Output:** A release checklist for `RELEASE-CHECKLIST.md`.

---

## S.7.7 Refactor vs Rebuild Rubric

**Prompt:**

> Create a refactor vs rebuild rubric for [COMPONENT]. Output criteria, scoring, and a recommendation. Include: test coverage, coupling, team familiarity, and business risk.

**Tired version:**

> Should I refactor or rebuild [COMPONENT]? Give me 5 criteria to decide.

**Output:** A decision rubric that prevents premature rewrites.

---

## S.7.8 Roadmap Next 5

**Prompt:**

> Propose a roadmap for [APP NAME]. Categorize features and rate them by value, risk, and complexity. Then propose a Next 5 sequence that is realistic and safe.

**Tired version:**

> Give me a Next 5 roadmap for [APP NAME].

**Output:** A prioritized roadmap.

---

## S.7.9 Retrofit Plan (Trust Without Rewrite)

**Prompt:**

> I have a messy KPI pipeline. Help me retrofit trust without a rewrite. Output a 7-step plan: define truth surface, add receipts, add health checks, add minimal contract, add tests at boundaries, add one alert, document handoff. Keep it tool-agnostic.

**Tired version:**

> List the top 5 hidden assumptions in this KPI and how to make each explicit.

**Output:** A retrofit plan that adds trust incrementally.

---

*For full context and when to use each prompt, see Appendix S in the Vibe Coding Bible.*
