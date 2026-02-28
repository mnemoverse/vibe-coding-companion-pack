# Prompt Library

> From: Vibe Coding Bible, Vol 1 — Appendix S

77 tool-agnostic prompts organized by workflow stage. Each prompt produces one artifact you can commit. Works with any AI coding tool.

**For Claude Code users:** These prompts are pre-configured as interactive, context-aware skills in the [vibe-coding-starter](https://github.com/mnemoverse/vibe-coding-starter) template. Skills know your project, run in phases, and evolve with your codebase.

| Section | Prompts | Focus |
|:--------|:-------:|:------|
| [S.1 Specification & Planning](s1-specification-planning.md) | 11 | Specs, domain rules, data shapes, edge cases |
| [S.2 Building & Features](s2-building-features.md) | 11 | Auth, CRUD, webhooks, RBAC, integrations |
| [S.3 Testing & Quality](s3-testing-quality.md) | 11 | Unit tests, smoke tests, property-based, flaky fixes |
| [S.4 Debugging](s4-debugging.md) | 9 | Evidence-first debugging, binary search, repro |
| [S.5 Security & Auth](s5-security-auth.md) | 9 | Threat models, OWASP, secrets, supply chain |
| [S.6 Deployment & Ops](s6-deployment-operations.md) | 11 | Deploy playbooks, incidents, rollbacks, runbooks |
| [S.7 Review & Refactoring](s7-review-refactoring.md) | 9 | Code review, diff summary, merge gates |
| [S.8 Incident Templates](s8-incident-templates.md) | 6 | Webhook backlog, double charge, account takeover |

## How to use

1. Find the prompt that matches what you're doing
2. Copy the prompt text
3. Replace `[PLACEHOLDERS]` with your project details
4. Paste into any AI tool (Claude, ChatGPT, Cursor, Copilot, etc.)

**Tired?** Each prompt has a shortened "tired version" for low-energy days.
