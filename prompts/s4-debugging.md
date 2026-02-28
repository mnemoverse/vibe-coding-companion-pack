# S.4: Debugging

> From: Vibe Coding Bible, Vol 1 — Appendix S
>
> Interactive skill version: [vibe-coding-starter](https://github.com/mnemoverse/vibe-coding-starter)

## S.4.1 Symptom to Facts

**Prompt:**

> I have a bug. Convert my description into:
> 1) Symptom (one sentence)
> 2) Expected behavior (one sentence)
> 3) Minimal repro steps (max 5 lines)
> 4) Unknowns (max 3)
> Then give ONE next evidence step that reduces uncertainty.
> Keep it calm and specific.

**Tired version:**

> "Convert this bug report into: symptom, expected, repro steps, one next step."

**Output:** A structured bug report that reduces panic.

---

## S.4.2 Hypotheses with Disproof Tests

**Prompt:**

> Here are the facts (symptom, repro, logs or stack trace).
> Generate exactly 3 hypotheses.
> For each hypothesis, give ONE fast disproof test and where to place the checkpoint.
> Do not suggest fixes yet.

**Tired version:**

> "3 hypotheses for this bug. One disproof test each. No fixes."

**Output:** Three testable hypotheses — the fastest path to root cause.

---

## S.4.3 Binary Search Checkpoints

**Prompt:**

> Here is the flow of the request and the boundaries.
> Suggest 3 binary search checkpoints that cut the space in half.
> For each checkpoint: what "good" looks like, what "bad" implies, and the next cut.

**Tired version:**

> "3 checkpoints to find where this breaks. Cut the space in half each time."

**Output:** A systematic search plan that avoids random poking.

---

## S.4.4 Minimal Repro Reducer

**Prompt:**

> Here is the full messy scenario.
> Reduce it to the smallest reproducible case.
> List which variables to freeze (data, timing, environment) and what I can remove first.
> Output only the minimal repro recipe and the freeze list.

**Tired version:**

> "Reduce this to the smallest repro. List what to freeze and what to remove."

**Output:** A minimal reproduction case that proves the bug exists.

---

## S.4.5 Log Schema (Safe by Default)

**Prompt:**

> I want structured logs for debugging.
> Propose the minimal set of boundary events and fields.
> Also list what must never be logged (privacy and security).
> Keep it tool-agnostic and minimal.

**Tired version:**

> "5 boundary events to log and 5 things to never log."

**Output:** A safe logging schema that helps debug without leaking.

---

## S.4.6 Production Plan Without Access

**Prompt:**

> I cannot reproduce locally.
> I have a production symptom and one snippet of evidence.
> Propose a plan using: metrics for scope, logs for story, traces for time if available, plus safe probes.
> For each step, tell me what evidence I should see if the hypothesis is correct.
> Keep it minimal and safe.

**Tired version:**

> "Plan to debug in production with only logs and metrics. No access to code."

**Output:** A safe production debugging plan.

---

## S.4.7 Fix Strategy Selector

**Prompt:**

> Proven cause: [paste]
> Risk context: [paste]
> Recommend a fix strategy: patch, guard, refactor, or revert.
> Explain why in 3 bullets, then propose the smallest change that addresses the cause.

**Tired version:**

> "Pick a fix strategy for this cause: patch, guard, refactor, or revert. One sentence why."

**Output:** A deliberate fix strategy instead of the first thing that compiles.

---

## S.4.8 Regression Lock Designer

**Prompt:**

> Given this bug and fix, design a regression lock.
> Pick the smallest reliable test or invariant, what it asserts, and what would make it flaky.

**Tired version:**

> "One regression test for this fix. What it asserts and what could make it flaky."

**Output:** A test that ensures this bug never comes back.

---

## S.4.9 Ship Safety Plan

**Prompt:**

> I am about to ship this fix.
> Write a minimal safety plan:
> 1) rollout scope (or the safest alternative if not possible)
> 2) what to watch (3 signals max)
> 3) what would trigger rollback or disable
> 4) the observation window
> Keep it short.

**Tired version:**

> "Ship plan: scope, 3 signals, rollback trigger. Keep it short."

**Output:** A confidence plan for shipping fixes safely.

---

*For full context and when to use each prompt, see Appendix S in the Vibe Coding Bible.*
