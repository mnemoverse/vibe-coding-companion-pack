# U.6: Automation Weekend

> From: Vibe Coding Bible, Vol 1 — Appendix U

*For: Adapted from Vol 5: Background Jobs & Scheduled Tasks.*

## 2h: Job Schema + Worker with Attempt Tracking

1. Design the job table: id, type, payload, status, attempts, max_attempts, created_at, next_run_at
2. Implement a simple worker that picks up pending jobs and processes them
3. Add attempt tracking: increment attempts on each run, mark failed after max_attempts
4. Run one job manually and verify the attempt count updates
5. Commit

**Done when:** You have a job queue with attempt tracking. One job ran successfully.

**Tired version:** Design the job schema. Write the migration. Think through the states: pending, running, completed, failed, dead.

## 6h: Queue Job + Scheduled Task + Dashboard

1. Complete the 2h plan
2. Add one queue job triggered by a user action (e.g., send welcome email after signup)
3. Add one scheduled job that runs on a cron (e.g., daily report, cleanup old sessions)
4. Build a simple dashboard showing: pending jobs, recent completions, recent failures
5. Write tests for: job creation, successful processing, failure after max attempts
6. Commit

**Done when:** One event-driven job and one scheduled job work. Dashboard shows their status.

## 12h: Full Automation with Reconciliation + Chaos Test

1. Complete the 6h plan
2. Add a dead-letter queue: jobs that fail permanently go here for human review
3. Add a reconciliation job: check that all expected scheduled jobs actually ran
4. Implement graceful shutdown: worker finishes current job before stopping
5. Run a chaos test: kill the worker mid-job, restart it, verify the job recovers
6. Add alerts for: dead-letter queue growing, scheduled job missed, worker not responding
7. Write a runbook: how to retry dead jobs, how to pause the queue, how to drain and restart
8. Commit and tag

**Done when:** Jobs recover from crashes. Dead letters are captured. Chaos test passes.

---

*For the philosophy behind time-boxed practice and the 2h/6h/12h format, see Appendix U in the Vibe Coding Bible.*
