# U.2: Building an MVP

> From: Vibe Coding Bible, Vol 1 — Appendix U

*For: Adapted from Vol 3: five themed weekends -- Contract / Build / Harden / Ship / Iterate.*

## 2h: Spec + One Core Feature

1. Write a product spec: who uses it, what it does, what it does not do
2. Define the single most important user action (the "golden path")
3. Build that one action end-to-end: UI to database and back
4. Commit the spec and the working feature

**Done when:** One user journey works from start to finish.

**Tired version:** Write just the spec. A good spec is worth a weekend by itself.

## 6h: Spec, Build, Test, Stage

1. Complete the 2h plan
2. Add the second most important feature
3. Write tests for both features (happy path + one failure case each)
4. Set up a staging environment and deploy
5. Walk through both features as a user would
6. Fix anything that breaks the flow
7. Commit

**Done when:** Two features work on staging. Tests pass. You can demo it.

## 12h: Ship with Observability

1. Complete the 6h plan
2. Add structured logging for key actions (user signed up, item created, error occurred)
3. Add a smoke test script that exercises the golden path automatically
4. Write a release checklist: what to verify before each deploy
5. Deploy to production
6. Run the smoke test against production
7. Set up one alert (error rate or downtime)
8. Commit and tag

**Done when:** App is live, smoke tests pass on production, you have one alert configured.

---

*For the philosophy behind time-boxed practice and the 2h/6h/12h format, see Appendix U in the Vibe Coding Bible.*
