# U.5: Integration Weekend

> From: Vibe Coding Bible, Vol 1 — Appendix U

*For: Adapted from Vol 4: Integration & Webhook Patterns.*

## 2h: Map Integrations + Webhook Receiver

1. List all external services your app talks to (payment, email, storage, etc.)
2. Pick the most important one and set up a webhook receiver endpoint
3. Implement signature verification on incoming webhooks
4. Log every received webhook with timestamp, type, and payload hash
5. Write one test: valid signature passes, invalid signature is rejected

**Done when:** You can receive a webhook, verify its signature, and log it.

**Tired version:** Map all integrations on paper. Draw the data flow. Know what talks to what.

## 6h: Inbox + Idempotent Handlers + Replay

1. Complete the 2h plan
2. Create a webhook inbox table: id, event type, payload, status, received_at, processed_at
3. Make handlers idempotent: processing the same event twice produces the same result
4. Add a replay mechanism: re-process a failed webhook from the inbox
5. Write tests for: duplicate event handling, failed event retry, inbox query
6. Commit

**Done when:** Webhooks are stored, processed idempotently, and can be replayed.

## 12h: Full Integration with Sync + Reconciliation

1. Complete the 6h plan
2. Add outbound integration: your app calls the external API (not just receiving)
3. Implement retry with exponential backoff for outbound calls
4. Build a reconciliation job: compare your local state with the external service's state, flag mismatches
5. Add a dashboard page showing: recent webhooks, processing status, reconciliation results
6. Write a runbook: what to do when the external service is down
7. Deploy and test with real webhooks (use the service's test mode)
8. Commit and tag

**Done when:** Bidirectional integration works. Reconciliation catches drift. Runbook covers outages.

---

*For the philosophy behind time-boxed practice and the 2h/6h/12h format, see Appendix U in the Vibe Coding Bible.*
