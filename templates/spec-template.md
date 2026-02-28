# Feature Specification Template

> From: Vibe Coding Bible, Vol 1 — Appendix K, Pattern 1

Write the spec before writing the prompt. This single practice eliminates most AI confusion and rework.

## Template

```markdown
# Feature Specification: [Name]

## What It Does
[One sentence describing the user-facing behavior]

## User Story
As a [type of user],
I want to [action],
So that [benefit].

## Inputs
- [Input 1]: [type, constraints]
- [Input 2]: [type, constraints]

## Outputs
- Success: [what happens]
- Failure: [what happens]

## Edge Cases
- [Edge case 1]: [expected behavior]
- [Edge case 2]: [expected behavior]

## Not Included
- [What this feature explicitly doesn't do]

## Technical Constraints
- [Performance requirements]
- [Compatibility requirements]
- [Security requirements]
```

---

*For a worked example (Password Reset) and how to feed specs into AI prompts, see Appendix K in the Vibe Coding Bible.*
