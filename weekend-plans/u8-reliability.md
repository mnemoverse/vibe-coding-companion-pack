# U.8: Reliability Weekend

> From: Vibe Coding Bible, Vol 1 — Appendix U

*For: Adapted from Vol 11: Reliability & Operational Readiness.*

## 2h: Health Check + SLO + One Alert

1. Add a health check endpoint: returns 200 when the app is healthy, includes database connectivity check
2. Define one SLO: "99% of requests complete in under 500ms" (or whatever fits your app)
3. Set up one alert that fires when the SLO is at risk (e.g., error rate > 1% for 5 minutes)
4. Verify the health check works and the alert fires when you simulate a failure
5. Commit

**Done when:** Health check returns real status. One SLO defined. One alert configured and tested.

**Tired version:** Write down your SLOs on paper. What promises are you making to users? Knowing this changes how you build.

## 6h: Structured Logs + Alert Ladder + Runbooks

1. Complete the 2h plan
2. Ensure all logs are structured (JSON with consistent fields)
3. Build an alert ladder with 3 levels:
   - Warning: error rate > 0.5% (notify via log)
   - Error: error rate > 2% (notify via chat/email)
   - Critical: service down > 2 min (page on-call)
4. Write 2 runbooks: one for "app is slow" and one for "app is down"
5. Each runbook has: symptoms, investigation steps, common fixes, escalation path
6. Commit

**Done when:** Alert ladder defined and configured. Two runbooks written with actionable steps.

## 12h: Full Reliability Baseline + Game Day Drill

1. Complete the 6h plan
2. Add circuit breakers for external service calls (fail fast instead of hanging)
3. Add graceful degradation: if a non-critical service is down, the app still works with reduced functionality
4. Run a game day drill:
   - Simulate database slowdown: does the alert fire? Does the runbook help?
   - Simulate external service outage: does the circuit breaker work? Does the app degrade gracefully?
   - Simulate high traffic: does the app stay within SLO?
5. Write up the game day results: what worked, what broke, what to improve
6. Fix the top issue found during game day
7. Commit and tag

**Done when:** Circuit breakers and graceful degradation work. Game day completed. Top issue fixed.

---

*For the philosophy behind time-boxed practice and the 2h/6h/12h format, see Appendix U in the Vibe Coding Bible.*
