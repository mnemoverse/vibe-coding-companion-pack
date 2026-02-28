# S.6: Deployment & Operations

> From: Vibe Coding Bible, Vol 1 — Appendix S
>
> Interactive skill version: [vibe-coding-starter](https://github.com/mnemoverse/vibe-coding-starter)

## S.6.1 Deploy Playbook

**Prompt:**

> Draft a deploy playbook for a small web app with a database. Include release sequence, migration safety rules, rollback strategy, and a post-deploy smoke test checklist. Tool-agnostic.

**Tired version:**

> Give me a deploy checklist with migrations and rollback steps.

**Output:** A deploy playbook for `DEPLOY-PLAYBOOK.md`.

---

## S.6.2 Incident Report Template

**Prompt:**

> Write a concise incident report template. Include timeline, impact, detection, root cause, remediation, and follow-ups. Keep it short and builder-friendly.

**Tired version:**

> Give me a short incident report template.

**Output:** An incident template you can fill in under stress.

---

## S.6.3 Rollback Plan

**Prompt:**

> Write a rollback plan for [DEPLOYMENT]. Include steps to revert, verification checks, and communication template.

**Tired version:**

> Write a basic rollback plan.

**Output:** A rollback plan you can execute at 2am.

---

## S.6.4 One-Page Readiness Review

**Prompt:**

> Create a one-page production readiness review for this release. Output sections: Changes, Top Risks, Evidence, Rollback, Monitoring Signals. Keep it short and specific.

**Tired version:**

> Make a release readiness checklist for this change with risks, evidence, rollback, and signals.

**Output:** A pre-release review document.

---

## S.6.5 Runbook Template

**Prompt:**

> Write a runbook for this incident: [describe incident]. Output numbered steps under headings: Symptom, Fast checks, Containment, Diagnosis, Fix forward, Rollback, Verification, Post-incident notes.

**Tired version:**

> Make a 10-step runbook for this incident with containment first.

**Output:** A runbook that works when you are stressed.

---

## S.6.6 Postmortem

**Prompt:**

> Turn these incident notes into a lightweight postmortem. Output sections: Summary, Impact, Detection, Timeline, Root Cause, Contributing Factors, What Worked, What Failed, Action Items. Keep tone calm and specific. Limit action items to two.

**Tired version:**

> Extract two action items from this incident. One detection improvement, one prevention improvement.

**Output:** A blameless postmortem with actionable follow-ups.

---

## S.6.7 On-Call Policy

**Prompt:**

> Create an on-call policy for a tiny team operating this app. Output: Severity definitions, Alert signals, Response expectations, Quiet hours rule, and a simple escalation plan.

**Tired version:**

> Give me a simple on-call policy with Sev 1, Sev 2, Sev 3 and what we do for each.

**Output:** An on-call policy that protects your sleep.

---

## S.6.8 Handoff Pack

**Prompt:**

> Generate a handoff pack outline for this app. Output a folder tree with filenames and one-sentence description for each file. Keep it under 12 files.

**Tired version:**

> List the 10 things a new owner needs in the first hour.

**Output:** A handoff package structure for `docs/`.

---

## S.6.9 Alert Policy (Low Noise)

**Prompt:**

> Design a low-noise alerting policy. Output: which checks can trigger alerts, suppression rules, what the alert message must include, and what the first response should be. Keep alerts scarce.

**Tired version:**

> Rewrite this alert message so it is actionable in 30 seconds.

**Output:** An alerting policy that you will not learn to ignore.

---

## S.6.10 Data Safety Baseline

**Prompt:**

> Design a data safety baseline for this app. Output sections: Backups, Restore procedure, Migration workflow, Undo stories for the top 3 data risks. Keep it small-team-friendly.

**Tired version:**

> Give me a data safety checklist with backups, restore, and migration rules.

**Output:** A data safety plan.

---

## S.6.11 Rescue Mode Plan

**Prompt:**

> I am in Rescue Mode. Given this symptom list, output the 10-minute rescue plan: containment, rollback decision, top checks, and one user communication message. Keep it calm.

**Tired version:**

> Rescue mode plan for these symptoms. Output only steps.

**Output:** A calm plan for when everything is on fire.

---

*For full context and when to use each prompt, see Appendix S in the Vibe Coding Bible.*
