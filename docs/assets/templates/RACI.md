# RACI / Responsibility Template

> Use this template when responsibility for a defined capability, process, decision, rule or data asset needs to be clarified. Do not use RACI as a substitute for stakeholder discovery.

## When to Use

Use a RACI when:

- responsibility is genuinely ambiguous;
- several teams participate in the same process;
- a control requires explicit accountability;
- ownership needs to be validated;
- a future operating model needs a clear decision.

Do not create a RACI merely because a project template expects one.

## RACI Definitions

- **R — Responsible:** performs or coordinates the work.
- **A — Accountable:** owns the outcome and has final accountability.
- **C — Consulted:** contributes expertise before the activity/decision.
- **I — Informed:** needs to know the outcome.

### DISCOVER Guidance

- Prefer **one Accountable role** where the business model permits it.
- If several roles appear Accountable, treat that as a discovery finding rather than forcing the table to look tidy.
- Use **roles**, not named individuals, in the durable artefact.
- Link the row to a stable DISCOVER ID such as `CAP-`, `PRC-`, `DEC-`, `BR-`, `DAT-` or `VAL-`.
- Where responsibility is not established, write `UNKNOWN`.
- Record evidence and validation status.

## Context

| Field | Value |
|---|---|
| Discovery / Domain | |
| Scope | |
| Business Outcome | |
| Prepared By | |
| Date | |
| Validation Owner | |
| Status | Unvalidated / Validated / Conflicted / Superseded |

## Responsibility Matrix

| DISCOVER ID | Capability / Process / Decision / Artefact | Role A | Role B | Role C | Role D | Evidence | Status / Notes |
|---|---|---|---|---|---|---|---|
| `PRC-001` | Example Process | A | R | C | I | `EVD-001` | Unvalidated |
| | | | | | | | |

## Accountability Questions

For each row ask:

1. Who is accountable for the outcome, not just the task?
2. Who actually performs the work today?
3. Who can approve an exception?
4. Who can change the relevant rule or definition?
5. Who must be consulted because of specialist knowledge or control responsibilities?
6. Who consumes the result and needs to be informed?
7. Does the documented responsibility match actual practice?
8. Is accountability end-to-end or fragmented across organisational boundaries?

## Decision-Rights Extension

For material decisions, use this supplementary view.

| Decision ID | Decision | Recommends | Decides | Approves / Overrides | Consulted | Informed | Evidence | Status |
|---|---|---|---|---|---|---|---|---|
| `DEC-001` | | | | | | | | |

## Ownership Extension

For data/semantic governance:

| Artefact ID | Asset / Definition / Rule | Business Owner | Steward / Maintainer | Technology Custodian | Validator | Evidence | Status |
|---|---|---|---|---|---|---|---|
| `INF-001` | | | | | | | |

## Conflicts / Gaps

| ID | Responsibility Conflict or Gap | Why It Matters | Evidence | Validation Needed | Owner |
|---|---|---|---|---|---|
| `OQ-001` | | | | | |

## Validation Checklist

- [ ] Roles are defined consistently.
- [ ] Actual practice has been compared with formal documentation.
- [ ] Accountable is distinguished from Responsible.
- [ ] Decision authority is explicit.
- [ ] Data/system ownership is not assumed to equal business ownership.
- [ ] Conflicts are visible rather than silently resolved.
- [ ] Rows link to supporting evidence.
- [ ] Relevant stakeholders have validated the result.
