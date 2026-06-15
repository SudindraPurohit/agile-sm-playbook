# Impediment Log & Escalation Framework

> **Facilitator note:** The impediment log is the SM's most important operational tool. An impediment that isn't written down doesn't get resolved — it just slows the team silently. Log everything. Escalate fast. Never sit on a blocker for more than 24 hours without an action.

---

## Impediment Log Template

Use this as a table in Confluence, a Jira epic, or a simple spreadsheet.

| ID | Raised By | Date Raised | Description | Impact | Owner | Status | Escalated To | Resolution | Date Resolved |
|----|-----------|-------------|-------------|--------|-------|--------|--------------|------------|---------------|
| IMP-001 | | | | | | Open | | | |
| IMP-002 | | | | | | In Progress | | | |

### Field definitions

- **Impact:** Low / Medium / High / Sprint-blocking
- **Status:** Open / In Progress / Escalated / Resolved / Accepted Risk
- **Escalated To:** Name of person or team the impediment was escalated to (SM, RTE, PO, Engineering Lead, etc.)

---

## Escalation Path

Use this decision tree when an impediment is raised:

```
IMPEDIMENT RAISED
       |
       v
Can the SM resolve it within 24 hours?
       |
      YES --> SM resolves. Log resolution. Done.
       |
       NO
       |
       v
Is it within the team's control?
       |
      YES --> Assign to team member. Timebox to 48 hours. Track daily.
       |
       NO
       |
       v
Is it a cross-team dependency or organisational blocker?
       |
      YES --> Escalate to:
              - Another SM (if cross-team)
              - RTE / Delivery Lead (if program-level)
              - PO (if business decision needed)
              Log escalation with date and owner.
       |
       NO
       |
       v
Is it a technical architecture or infrastructure issue?
       |
      YES --> Escalate to Engineering Lead / Architect
              Create a spike if discovery is needed
       |
       v
Is it unresolvable in this sprint?
       |
      YES --> Document as Accepted Risk
              Communicate impact to PO and stakeholders
              Add mitigation plan to next sprint planning
```

---

## Escalation SLAs (recommended)

| Impediment Type | Expected Resolution Time | Escalation Trigger |
|---|---|---|
| Low impact, within team | 3 days | Escalate if unresolved after 3 days |
| Medium impact, cross-team | 2 days | Escalate immediately to relevant SM/lead |
| High impact, sprint-blocking | Same day | Escalate within 2 hours of identification |
| Organisational / policy blocker | 1 sprint | Flag to RTE/management immediately |

---

## Common impediment categories

- **Environment issues** — dev/test/staging environments unavailable or broken
- **Dependency blockers** — waiting on another team's API, data, or sign-off
- **Unclear requirements** — stories lack sufficient detail to develop against
- **Resource constraints** — key team member unavailable (leave, pulled to another project)
- **Technical blockers** — architecture decisions unmade, access not provisioned
- **Process blockers** — approval gates, compliance reviews, change management delays

---

## SM Tips

- Raise impediments in Daily Scrum but do not solve them there — take them offline
- Never normalise impediments. "We always wait 3 days for environment access" is an impediment, not just how things work
- Track resolution time as a metric — average impediment age tells you how healthy your escalation path is
- At the end of each sprint, review resolved impediments in retrospective: *"What systemic changes would prevent these from recurring?"*
