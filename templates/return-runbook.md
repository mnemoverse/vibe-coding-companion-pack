# Return Runbook Template

> From: Vibe Coding Bible, Vol 1 — Appendix N

For projects with integrations, background jobs, or external dependencies. Use this checklist when returning to a project after a gap.

## Template

```markdown
## Return Runbook

1. Read HANDOFF-NOTE.md and restate the contract in your own words
2. Run the project locally — does it start?
3. Run tests — do they pass?
4. Open logs — any recent errors?
5. Check external dependencies — any changelog notices?
6. Choose one small improvement tied to a recent issue
7. Ship using the standard deploy process
```

## When to use

- **Returning from vacation** — run it yourself before diving into code
- **Onboarding a new team member** — they follow this to start contributing
- **After a long gap** — when you can't remember how things work

## Maintenance

- Update weekly if anything changed (two minutes)
- Before vacation: run it yourself to verify it works
- If you cannot follow your own runbook, nobody else can either

---

*For the handoff note template, team collaboration models, and shared context management, see Appendix N in the Vibe Coding Bible.*
