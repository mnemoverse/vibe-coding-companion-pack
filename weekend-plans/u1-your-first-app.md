# U.1: Your First App

> From: Vibe Coding Bible, Vol 1 — Appendix U

*For: Someone who has never shipped anything with AI tools.*

## 2h: One Visible Slice

1. Choose your tool (Cursor, Claude Code, or Lovable)
2. Create a project folder, initialize git, write a one-paragraph spec
3. Prompt the AI: "Build a [simple thing] that does [one action]"
4. Get it running locally -- you should see something on screen
5. Commit

**Done when:** You can show someone a working screen and say "I built this."

**Tired version:** Open Lovable, describe a to-do list app, click deploy. You shipped.

## 6h: Full Feature with Tests

1. Complete the 2h plan
2. Add one more feature (search, filtering, or a second page)
3. Write 3 tests: one happy path, one edge case, one error case
4. Fix any bugs the tests reveal
5. Deploy to a staging URL (Vercel, Netlify, or Lovable's built-in hosting)
6. Commit and tag: `v0.1.0`

**Done when:** Someone can visit a URL and use your app. Tests pass.

## 12h: Ship MVP to Production

1. Complete the 6h plan
2. Add error handling for every user-facing action
3. Add basic monitoring: console errors logged, health check endpoint
4. Write a one-page README: what it does, how to run it, how to deploy
5. Deploy to production URL with a real domain (or subdomain)
6. Send the link to one real person and ask them to use it
7. Commit and tag: `v1.0.0`

**Done when:** A real person used your app and you have their feedback.

---

*For the philosophy behind time-boxed practice and the 2h/6h/12h format, see Appendix U in the Vibe Coding Bible.*
