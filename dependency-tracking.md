# Cross-Team Dependency Tracking Framework

> **Facilitator note:** Dependencies are the silent killers of sprint predictability. Most teams discover them too late — during execution rather than planning. This framework gives you a structured way to surface, track, and resolve dependencies before they become blockers.

---

## Dependency Register Template

| DEP-ID | Dependent Team | Providing Team | Description | Needed By (Sprint/Date) | Status | Owner | Risk If Delayed | Notes |
|--------|---------------|----------------|-------------|------------------------|--------|-------|-----------------|-------|
| DEP-001 | | | | | Identified | | | |
| DEP-002 | | | | | Confirmed | | | |
| DEP-003 | | | | | At Risk | | | |
| DEP-004 | | | | | Resolved | | | |

### Status definitions
- **Identified** — dependency exists but not yet confirmed with providing team
- **Confirmed** — providing team has acknowledged and committed to delivery date
- **At Risk** — delivery date in doubt; escalation may be needed
- **Blocked** — dependency is actively blocking work; immediate escalation required
- **Resolved** — dependency delivered and consumed

---

## Dependency Identification Checklist

Run this during backlog refinement for every story above medium complexity:

- [ ] Does this story rely on an API, data feed, or service owned by another team?
- [ ] Does this story require a decision or sign-off from outside the team?
- [ ] Does this story share a component, environment, or release with another team?
- [ ] Does another team's story need to be completed before this one can start?
- [ ] Are there compliance, legal, or architecture reviews required?

If any answer is YES — log it as a dependency immediately.

---

## Dependency Review Cadence

| When | What to review |
|------|----------------|
| Backlog Refinement | Identify new dependencies for upcoming stories |
| Sprint Planning | Confirm all dependencies for committed stories are resolved or have clear owners |
| Daily Scrum | Surface any dependencies that have become blockers overnight |
| Cross-team Sync (weekly) | Review At Risk and Blocked dependencies with other SMs or leads |
| Sprint Review | Note any dependencies that caused delivery delays — feed into retrospective |

---

## Visualising Dependencies

For program-level dependency mapping, use a simple board with three swim lanes:

```
+------------------+------------------+------------------+
|   TEAM A NEEDS   |   IN PROGRESS    |   TEAM B NEEDS   |
|   FROM TEAM B    |                  |   FROM TEAM A    |
+------------------+------------------+------------------+
|                  |                  |                  |
|  [DEP-001]       |  [DEP-003]       |  [DEP-002]       |
|  API endpoint    |  UAT data set    |  Auth token      |
|  Needed: Sp 4    |  Owner: Team B   |  Needed: Sp 3    |
|                  |  Due: Nov 12     |                  |
+------------------+------------------+------------------+
```

This visual works in Miro, Confluence, or a physical board. Update it at every cross-team sync.

---

## When a dependency becomes a blocker

1. Flag it in the same-day standup — do not wait
2. SM contacts the providing team's SM directly
3. If unresolved within 24 hours — escalate to delivery lead or RTE
4. Document the business impact: *"This dependency is blocking Story X, which is worth Y story points and is on the critical path to Sprint Goal Z"*
5. Explore parallel options — can the dependent story be de-scoped or resequenced?
