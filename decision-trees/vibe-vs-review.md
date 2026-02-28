# When to Vibe vs. Review

> From: Vibe Coding Bible, Vol 1 — Appendix P

## Should I Let AI Run or Review Each Step?

```text
How well do I understand this area?
|
+-- NOT AT ALL
|   |
|   +-- --> REVIEW EACH STEP
|       Learn from AI, verify as you go
|
+-- SOMEWHAT
|   |
|   +-- How critical is this code?
|       |
|       +-- LOW (experimental, can redo)
|       |   --> LET AI RUN
|       |
|       +-- MEDIUM (feature, has tests)
|       |   --> REVIEW SUMMARIES
|       |   Let AI work, review what it did
|       |
|       +-- HIGH (security, core logic)
|           --> REVIEW EACH STEP
|
+-- DEEPLY
    |
    +-- Is this tedious or interesting?
        |
        +-- TEDIOUS (boilerplate, repetitive)
        |   --> LET AI RUN
        |
        +-- INTERESTING (novel, architectural)
            --> REVIEW EACH STEP
            Your judgment adds value
```

## Quick Matrix

| Understanding | Criticality | Approach |
|--------------|-------------|----------|
| Low | Low | Review each step (learning opportunity) |
| Low | High | Review each step (risk management) |
| High | Low | Let AI run (efficient) |
| High | High | Review summaries (trust but verify) |

---

*For tool and platform selection trees, see Appendix H. For stack and framework selection, see Appendix K. For full context, see Appendix P in the Vibe Coding Bible.*
