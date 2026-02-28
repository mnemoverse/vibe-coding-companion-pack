# U.10: Create Your Own Weekend Plan (Meta-Template)

> From: Vibe Coding Bible, Vol 1 — Appendix U

*For: Use this template to design a weekend build plan for any goal.*

## Step 1: Define the Goal

Write one sentence: "By the end of this weekend, I want to ___."

## Step 2: Break It into 2h / 6h / 12h

**2h scope:** What is the smallest useful thing? The thing you could finish even when tired?

- One action, one visible result, one commit.
- This is your tired version. It should feel easy enough that you never skip it.

**6h scope:** What adds real substance? Tests, a second feature, staging deploy?

- The 2h work plus 2-3 more steps.
- Should feel like a solid half-day of work.

**12h scope:** What makes it shippable? Monitoring, production deploy, documentation?

- The 6h work plus production readiness.
- Should feel like "I could hand this to someone else."

## Step 3: Define "Done"

For each version, write one sentence: "Done when ___."

Be specific. "Done when the health check returns real database status" is better than "Done when monitoring is set up."

## Step 4: Write the Tired Version

The tired version is the most important part. It should be:

- Completable in under 2 hours, even on a bad day
- Useful on its own, not just setup for the 6h version
- Satisfying enough that you feel good about finishing

## Template

```markdown
## [Plan Name]

*Goal: [One sentence]*

### 2h: [Short description]

1. [Step]
2. [Step]
3. [Step]

**Done when:** [Specific outcome]

**Tired version:** [Even shorter version of the 2h plan]

### 6h: [Short description]

1. Complete the 2h plan
2. [Step]
3. [Step]
4. [Step]

**Done when:** [Specific outcome]

### 12h: [Short description]

1. Complete the 6h plan
2. [Step]
3. [Step]
4. [Step]
5. [Step]

**Done when:** [Specific outcome]
```

## Example: Custom Plan for Adding Search

```markdown
## Search Feature Weekend

*Goal: Users can search through their content and get results in under 200ms.*

### 2h: Basic Search

1. Add a search input to the main page
2. Implement server-side full-text search on the title field
3. Return results and display them
4. Write one test: search for a known item returns it

**Done when:** Searching for a title returns matching results.

**Tired version:** Just add the search input and wire it to a LIKE query. Works for small datasets.

### 6h: Smart Search + Tests

1. Complete the 2h plan
2. Add full-text search on title AND body fields
3. Add search result ranking (relevance scoring)
4. Add debounced search-as-you-type
5. Write tests for: no results case, special characters, relevance ordering
6. Measure search latency and record it

**Done when:** Search works on all fields with ranking. Latency measured. Tests pass.

### 12h: Production Search

1. Complete the 6h plan
2. Add search index (database full-text index or dedicated search service)
3. Add search analytics: what do users search for? What returns no results?
4. Set a performance budget: search must return in under 200ms at P95
5. Add a performance test that verifies the budget
6. Deploy and verify search works in production
7. Write a runbook: how to rebuild the search index

**Done when:** Search is indexed, fast, and observable. Performance budget enforced. Production verified.
```

---

*For the philosophy behind time-boxed practice and the 2h/6h/12h format, see Appendix U in the Vibe Coding Bible.*
