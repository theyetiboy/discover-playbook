---
title: Golden Thread Traceability
version: 1.0
---

# Golden Thread Traceability Matrix

> Connect business strategy to measurable value using evidence-supported relationships.

## Golden Thread

**Business Strategy**
→ **Business Capability**
→ **Business Process**
→ **Business Decision**
→ **Business Information**
→ **Business Rules**
→ **Technology / Data**
→ **Data Product / Analytics**
→ **Insight / Action**
→ **Business Value**

## Traceability Matrix

| Strategy | Capability | Process | Decision | Information | Rule | System / Data | Product / Analytics | Action | Value | Evidence | Relationship Status |
|---|---|---|---|---|---|---|---|---|---|---|---|
| STR- | CAP- | PRC- | DEC- | INF- | BR- | SYS- / DAT- | DP- | ACT- | VAL- | EVD- | |

Use multiple rows where relationships branch.

Do not force artificial one-to-one relationships.

## Relationship Register

| From ID | Relationship | To ID | Evidence | Status | Confidence | Validation Needed |
|---|---|---|---|---|---|---|
| CAP- | enables / contains / depends on / other | PRC- | EVD- | Unvalidated | | |

## Broken Thread Register

| Gap ID | From | Missing / Weak Link | To | Why It Matters | Evidence Needed | Owner |
|---|---|---|---|---|---|---|
| BT-001 | DEC- | Information requirement unknown | INF- | | | |

`BT-` is a local gap identifier for this matrix and does not represent a permanent business object.

## Traceability Status

Suggested values:

- Validated
- Unvalidated
- Conflicted
- Unknown

## Quality Checks

- [ ] Business outcome identified
- [ ] Relevant capability identified
- [ ] Process identified where relevant
- [ ] Decision identified
- [ ] Decision owner identified or marked unknown
- [ ] Information requirement identified
- [ ] Business rules identified where relevant
- [ ] Systems / data connected where relevant
- [ ] Candidate product or analytics connected to a real decision/action
- [ ] Business action identified
- [ ] Value / success measure identified
- [ ] Evidence attached to material relationships
- [ ] Broken Thread gaps visible
- [ ] Stakeholders have validated material relationships

## Guidance

- A blank or `UNKNOWN` link is preferable to an invented relationship.
- Preserve existing IDs.
- Record conflicting relationships rather than silently selecting one.
- A candidate data product with no identifiable consumer, decision, action or value should be challenged.
