# Definition of Ready (DoR) Checklist

> **Facilitator note:** The DoR is your quality gate before Sprint Planning. If a story doesn't meet DoR, it does not enter the sprint — no exceptions. This protects the team from mid-sprint discoveries that blow up estimates. The PO owns DoR compliance; the SM enforces it at the planning gate.

---

## What is the Definition of Ready?

A story is "ready" when the team has enough information to confidently commit to it, estimate it, and deliver it within a single sprint without needing to go back to the PO for fundamental clarifications.

---

## DoR Checklist — Standard Template

### Story Clarity
- [ ] User story written in standard format: *"As a [user], I want [action] so that [benefit]"*
- [ ] Business value is clearly stated — the team understands *why* this matters
- [ ] Scope is clear — what is explicitly IN and OUT of this story is defined

### Acceptance Criteria
- [ ] At least 3 acceptance criteria defined
- [ ] Acceptance criteria are testable (can be verified with a pass/fail outcome)
- [ ] Edge cases and error scenarios are documented
- [ ] No ambiguous language ("fast", "user-friendly", "better") without measurable definition

### Dependencies
- [ ] All external dependencies identified
- [ ] Dependent teams or systems have been notified and have confirmed availability
- [ ] Any API contracts, data requirements, or environment needs are confirmed

### Estimation
- [ ] Story has been estimated by the team (story points or t-shirt size)
- [ ] Story fits within a single sprint (if not, it has been split)
- [ ] Team has flagged any technical uncertainty or spike needed

### Design & UX (if applicable)
- [ ] Designs or wireframes attached and reviewed by the team
- [ ] Design has PO sign-off before sprint start

---

## DoR Quick Reference Card

Use this at the end of every refinement session:

```
STORY: ________________________________

[ ] Has a clear user story format
[ ] Has testable acceptance criteria (3+)
[ ] Dependencies identified and confirmed
[ ] Estimated by the team
[ ] Fits in one sprint
[ ] PO can answer questions about it without going back to stakeholders

READY? YES / NO
If NO — reason: ________________________________
Target ready date: ________________________________
```

---

## How to handle stories that fail DoR at planning

1. Do not let the story enter the sprint
2. Document specifically what is missing
3. Assign the PO an action to resolve it before the next planning
4. If the team is regularly failing DoR at planning, the refinement process needs fixing — raise it in the next retrospective
