# U.7: Debugging Sprint

> From: Vibe Coding Bible, Vol 1 — Appendix U

*For: Adapted from Vol 10: Systematic Debugging.*

## 2h: Bug Notebook + Boundary Logs + Practice Run

1. Create a bug notebook (markdown file or note): date, symptom, hypothesis, actual cause, fix, lesson
2. Add 5 boundary logs to your app: one at each major boundary (API entry, database call, external service call, cache hit/miss, error handler)
3. Trigger one bug (or find one in your backlog) and walk through it using only the logs
4. Record the bug in your notebook with the full cycle: symptom, hypothesis, investigation, fix
5. Commit the logs and the notebook

**Done when:** You have boundary logs and one documented bug investigation.

**Tired version:** Create the bug notebook and write down your last 3 bugs from memory. Pattern recognition starts with recording.

## 6h: Structured Logs + Request ID + 3 Bug Patterns

1. Complete the 2h plan
2. Switch to structured logging (JSON format): every log has timestamp, level, message, and context
3. Add a request ID that flows through the entire request lifecycle
4. Find and fix 3 bugs using the structured logs (real bugs from your backlog)
5. Record all 3 in the bug notebook
6. Look for patterns: are they all in the same area? Same type of mistake?
7. Commit

**Done when:** Structured logs with request IDs. 3 bugs documented with patterns identified.

## 12h: Correlation IDs + Health Dashboard + Incident Drill

1. Complete the 6h plan
2. Add correlation IDs that connect related operations across services (or across background jobs and API requests)
3. Build a health dashboard: request count, error rate, P95 latency, recent errors
4. Run an incident drill: simulate a production issue (database down, external service timeout), use your logs and dashboard to diagnose it, write up the incident
5. Add the incident report to your bug notebook
6. Write a runbook: how to investigate common failure modes using your observability stack
7. Commit and tag

**Done when:** Correlation IDs trace across boundaries. Dashboard shows system health. Incident drill completed.

---

*For the philosophy behind time-boxed practice and the 2h/6h/12h format, see Appendix U in the Vibe Coding Bible.*
