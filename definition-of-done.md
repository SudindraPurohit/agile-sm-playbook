# Definition of Done (DoD) Checklist

> **Facilitator note:** The DoD is a shared agreement, not an SM diktat. This template should be reviewed with the team in the first sprint and adapted to fit your context. Revisit it every 3–4 sprints in retrospective. A DoD that never changes is a DoD the team has stopped thinking about.

---

## What is the Definition of Done?

The DoD is the team's shared understanding of what "complete" means for any piece of work. A story is not done when development is finished — it is done when every item on this list is satisfied.

---

## DoD Checklist — Standard Template

### Code Quality
- [ ] Code written and peer-reviewed (minimum 1 reviewer)
- [ ] Code follows agreed naming conventions and style guide
- [ ] No commented-out code left in the codebase
- [ ] Technical debt created (if any) is logged as a backlog item

### Testing
- [ ] Unit tests written and passing (minimum coverage threshold met)
- [ ] Integration tests updated where applicable
- [ ] Regression suite run and passing
- [ ] Exploratory testing completed by QA
- [ ] No open P1 or P2 defects related to this story

### Acceptance Criteria
- [ ] All acceptance criteria from the story verified and signed off
- [ ] Edge cases identified during refinement have been tested
- [ ] Product Owner has reviewed and accepted the story

### Documentation
- [ ] Release notes updated (if user-facing change)
- [ ] API documentation updated (if applicable)
- [ ] Confluence / wiki page updated if process or architecture changed

### Deployment
- [ ] Code merged to main/release branch
- [ ] Build pipeline passing (no broken builds)
- [ ] Deployed to staging/UAT environment
- [ ] Smoke test passed post-deployment

---

## DoD for Bug Fixes (Simplified)

- [ ] Root cause identified and documented
- [ ] Fix implemented and code reviewed
- [ ] Unit test added to prevent regression
- [ ] Verified in the environment where the bug was reported
- [ ] Linked to original defect ticket and closed

---

## How to use this with your team

1. Present this as a starting draft in Sprint 0 or your first retrospective
2. Ask: *"Is there anything here we can't commit to yet? Is there anything missing that matters to us?"*
3. Agree on the final version as a team — document it in Confluence or pin it to your Jira board
4. Review it every quarter in retrospective — ask: *"Is our DoD making us better, or is it just a checkbox exercise?"*

---

## Common DoD anti-patterns to watch for

| Anti-pattern | What it looks like | Fix |
|---|---|---|
| DoD ignored under pressure | "We'll skip the regression this sprint, we're behind" | Hold the line — a story is not done. Log the risk explicitly. |
| DoD too vague | "Code is clean" | Make it measurable: "Code reviewed by at least 1 team member" |
| DoD too strict for current maturity | Team fails DoD every sprint | Calibrate to current capability, improve incrementally |
| PO not involved in sign-off | Stories closed without PO review | Add PO acceptance as a hard gate, not optional |
