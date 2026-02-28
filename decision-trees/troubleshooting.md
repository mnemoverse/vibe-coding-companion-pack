# Troubleshooting Decisions

> From: Vibe Coding Bible, Vol 1 — Appendix P

## Should I Reset Context?

```text
Is AI giving poor responses?
|
+-- NO --> Continue
|
+-- YES
    |
    +-- Have you been talking for 50+ messages?
        |
        +-- YES --> RESET (context pollution likely)
        |
        +-- NO
            |
            +-- Has AI started forgetting earlier instructions?
                |
                +-- YES --> RESET
                |
                +-- NO
                    |
                    +-- Are responses getting worse over time?
                        |
                        +-- YES --> RESET
                        |
                        +-- NO --> Problem is prompt, not context
```

## Should I Restart the Project?

```text
Are you making progress?
|
+-- YES --> Continue
|
+-- NO
    |
    +-- Is the architecture fundamentally wrong?
        |
        +-- YES --> RESTART
        |   Capture lessons, start fresh
        |
        +-- NO
            |
            +-- Have you been debugging the same issue for hours?
                |
                +-- YES
                |   |
                |   +-- Tried 3+ different approaches?
                |       |
                |       +-- YES --> RESTART that component
                |       |
                |       +-- NO --> Try different approach first
                |
                +-- NO --> Continue with fresh context
```

## Is This a Fix Loop or Normal Iteration?

```text
How many times have you tried to fix this specific issue?
|
+-- 1-2 --> Normal iteration, continue
|
+-- 3-4 --> Warning zone
|   |
|   +-- Are you trying the same type of fix?
|       |
|       +-- YES --> You're in a fix loop
|       |   STOP. Try completely different approach.
|       |
|       +-- NO --> Continue, but set timer (15 min max)
|
+-- 5+ --> You're definitely in a fix loop
    |
    +-- STOP. REVERT. RESTART.
```

---

*For anti-patterns and escape protocols, see Appendix L. For full context, see Appendix P in the Vibe Coding Bible.*
