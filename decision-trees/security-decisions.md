# Security Decisions

> From: Vibe Coding Bible, Vol 1 — Appendix P

## Should I Trust This AI-Generated Code?

```text
What type of code is this?
|
+-- SECURITY-SENSITIVE (auth, payments, data)
|   |
|   +-- --> FULL REVIEW REQUIRED
|       Use the AI Code Review checklist
|
+-- USER-FACING (inputs, outputs)
|   |
|   +-- --> CHECK FOR VULNERABILITIES
|       - Input validation
|       - Output encoding
|       - Error handling
|
+-- INTERNAL LOGIC
|   |
|   +-- --> TEST THOROUGHLY
|       - Unit tests for edge cases
|       - Integration tests for connections
|
+-- UTILITY / HELPER
    |
    +-- --> BASIC REVIEW
        - Does it work?
        - Is it simple?
```

## Should I Add This Dependency?

```text
Did AI suggest a dependency?
|
+-- Does it exist? (npm/pypi search)
    |
    +-- NO --> Don't use it (hallucination)
    |
    +-- YES
        |
        +-- Is it from a trusted source?
            |
            +-- NO/UNSURE --> Research carefully or skip
            |
            +-- YES
                |
                +-- Do you actually need it?
                    |
                    +-- Could write it yourself in <50 lines?
                    |   |
                    |   +-- YES --> Write it yourself
                    |   |
                    |   +-- NO --> Consider adding
                    |
                    +-- Is it actively maintained?
                        |
                        +-- NO --> Find alternative
                        |
                        +-- YES --> Check for vulnerabilities (npm audit)
                            |
                            +-- Clean? --> Add it
```

---

*For the full AI Code Review Checklist, see the [checklists](../checklists/) directory. For vulnerability patterns and code examples, see Appendix M in the Vibe Coding Bible.*
