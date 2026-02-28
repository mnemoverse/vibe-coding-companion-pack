# Project Kickoff

> From: Vibe Coding Bible, Vol 1 — Appendix P

## How Should I Start This Project?

```text
What stage is your idea?
|
+-- VAGUE ("I want to build something like...")
|   |
|   +-- --> Start with CONVERSATION
|       1. Open Claude.ai or ChatGPT
|       2. Describe your idea in plain English
|       3. Ask: "What questions should I answer before building this?"
|       4. Iterate until you have a clear spec
|       5. THEN choose tools
|
+-- CLEAR IDEA, NO SPEC ("I know what I want but haven't written it down")
|   |
|   +-- --> Create a SPEC FIRST
|       1. Open chat interface
|       2. Ask: "Help me write a product spec for [idea]"
|       3. Cover: who uses it, what it does, what it doesn't do
|       4. Save the spec in your project folder
|       5. Reference it in every prompt
|
+-- HAVE SPEC, NEED PROTOTYPE ("I know exactly what to build")
|   |
|   +-- --> Jump to BUILD
|       No code experience? --> Lovable or Bolt.new
|       Some experience? --> Cursor
|       Terminal comfortable? --> Claude Code
|
+-- HAVE PROTOTYPE, NEED PRODUCTION ("It works, needs polish")
    |
    +-- --> Focus on QUALITY
        1. Add tests (AI writes tests, you verify assertions)
        2. Security review (use the AI Code Review checklist)
        3. Error handling and edge cases
        4. Deploy to real environment
```

## First 30 Minutes of Any Project

```text
START
|
+-- 1. Create project folder
|   +-- mkdir project-name && cd project-name
|
+-- 2. Initialize git
|   +-- git init
|
+-- 3. Create CLAUDE.md (or .cursorrules)
|   |
|   +-- Include:
|       - What you're building (1 sentence)
|       - Tech stack
|       - Key constraints
|       - Commands (how to run/test)
|
+-- 4. First commit
|   +-- git add . && git commit -m "project setup"
|
+-- 5. Write first test (even before code)
|   |
|   +-- What's the ONE thing that must work?
|       Write a test for that. Just one.
|
+-- 6. Ask AI to make test pass
|   +-- "Implement the minimum code to make this test pass"
|
+-- 7. Commit working state
    +-- git commit -m "first working feature"

REPEAT 5-7 until MVP is done.
```

## When to Stop Building and Ship

```text
Are users waiting for this?
|
+-- YES
|   |
|   +-- Does the core feature work?
|       |
|       +-- YES --> SHIP IT
|       |   Polish later. Real feedback > imagined perfection.
|       |
|       +-- NO --> Keep building core only
|           Ignore nice-to-haves until core works
|
+-- NO (personal project / learning)
    |
    +-- Have you learned what you wanted to learn?
        |
        +-- YES --> SHIP IT OR MOVE ON
        |   The goal was learning. You achieved it.
        |
        +-- NO --> Keep building, but set a deadline
            "I'll ship whatever I have by [date]"
```

---

*For detailed first-week plans and tool setup, see Appendix H. For the Spec Template, see the [templates](../templates/) directory. For full context, see Appendix P in the Vibe Coding Bible.*
