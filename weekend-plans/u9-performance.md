# U.9: Performance Weekend

> From: Vibe Coding Bible, Vol 1 — Appendix U

*For: Adapted from Vol 12: Performance Budgets & Optimization.*

## 2h: Pick a Journey + Write a Budget + Create a Chart

1. Choose the most important user journey (e.g., "load dashboard" or "submit form")
2. Measure it: how long does it take right now? (Use browser devtools or server timing)
3. Write a performance budget: "This journey must complete in under X ms"
4. Create a simple chart or table: current time vs. budget vs. breakdown by phase
5. Commit the budget document

**Done when:** One journey measured. Budget written. You know where the time goes.

**Tired version:** Just measure one journey and write down the number. You cannot improve what you have not measured.

## 6h: Fix One Bottleneck with Before/After Proof

1. Complete the 2h plan
2. Identify the biggest bottleneck in the journey (slowest phase from your breakdown)
3. Fix it. Common fixes:
   - Add an index to a slow database query
   - Cache a repeated computation
   - Reduce payload size
   - Defer non-critical work to a background job
4. Measure again: create a before/after comparison
5. Write tests that verify the fix works (not just that it is fast -- regression tests)
6. Commit with the before/after numbers in the commit message

**Done when:** One bottleneck fixed. Before/after proof documented. Tests pass.

## 12h: Performance Gate + Rescue Pack + Weekly Habit

1. Complete the 6h plan
2. Add a performance gate to CI: if the journey exceeds the budget, the build fails
3. Build a "rescue pack" -- a documented set of quick wins you can apply when performance degrades:
   - Query optimization patterns that work for your schema
   - Caching strategies with cache-key conventions
   - Payload reduction techniques
4. Fix a second bottleneck using the rescue pack
5. Set up a weekly performance check: every Monday, run the journey measurement and compare to budget
6. Write a runbook: what to do when performance degrades (investigation steps, rescue pack reference, escalation)
7. Commit and tag

**Done when:** Performance gate in CI. Rescue pack documented. Weekly habit established. Two bottlenecks fixed.

---

*For the philosophy behind time-boxed practice and the 2h/6h/12h format, see Appendix U in the Vibe Coding Bible.*
