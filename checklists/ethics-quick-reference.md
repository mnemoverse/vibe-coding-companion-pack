# Ethics Quick Reference

> From: Vibe Coding Bible, Vol 1 — Appendix E

## Before Using AI

| Check | Question | If No |
|-------|----------|-------|
| [ ] | Is this task appropriate for AI? | Don't use AI |
| [ ] | Do I understand what I'm asking for? | Learn first |
| [ ] | Can I verify the output? | Get help or don't use |
| [ ] | Are there IP/confidentiality concerns? | Check with legal |
| [ ] | What's the risk if AI is wrong? | Add safeguards |

## During AI Use

| Check | Question | If No |
|-------|----------|-------|
| [ ] | Do I understand each line? | Ask AI to explain |
| [ ] | Am I maintaining my skills? | Do some manually |
| [ ] | Is the code secure? | Security review |
| [ ] | Does it match our patterns? | Adapt to codebase |
| [ ] | Am I just accepting blindly? | Slow down |

## After AI Use

| Check | Question | If No |
|-------|----------|-------|
| [ ] | Was expert review done (if needed)? | Get review |
| [ ] | Are there tests? | Write tests |
| [ ] | Is there an audit trail? | Document decisions |
| [ ] | Who's accountable? | Assign owner |
| [ ] | Can we roll back? | Create rollback plan |

## The 5-Second Ethics Test

Before accepting any AI suggestion:

1. **Would I be embarrassed if this broke?**
2. **Could this hurt a user?**
3. **Do I understand it?**
4. **Is there a simpler way?**
5. **Am I the right person to approve this?**

If any answer is concerning: **STOP and think.**

## Quick Reference Cards

### Card 1: Legal Quick Guide

```text
OWNERSHIP:
+-- Pure AI output --> No copyright
+-- Human-edited --> Probably protected
+-- Human-directed --> Usually protected
+-- When in doubt --> Document your contribution

RISK:
+-- Core IP --> Don't use pure AI
+-- Trade secrets --> Manual review
+-- Open source --> Check licenses
+-- Customer data --> Privacy review
```

### Card 2: Responsibility Quick Guide

```text
WHO'S RESPONSIBLE?
+-- No review done --> You
+-- Review missed it --> Reviewer
+-- Process failure --> Management
+-- Everyone followed process --> Company
+-- Vendor bug --> Company (then vendor claim)

PROTECT YOURSELF:
+-- Always review AI code
+-- Document your reviews
+-- Flag concerns in writing
+-- Follow the process
```

### Card 3: Daily Ethics

```text
BEFORE:
+-- Right task for AI?
+-- Can I verify?
+-- What if wrong?

DURING:
+-- Understanding code?
+-- Maintaining skills?
+-- Checking security?

AFTER:
+-- Reviewed properly?
+-- Tests written?
+-- Owner assigned?
```

---

*For the full ethics framework including IP law, accountability matrices, skill atrophy assessment, and the Professional's Oath, see Appendix E in the Vibe Coding Bible.*
