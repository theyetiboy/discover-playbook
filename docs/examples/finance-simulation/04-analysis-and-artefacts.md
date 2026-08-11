# Finance Simulation — Analysis and Artefacts

> Derived only from the synthetic workshop notes in this example.

## Executive Summary

The workshop supports the view that Finance experiences material manual reconciliation and terminology inconsistency around forecast and recognised revenue. It also identifies important decisions and a candidate recognition rule.

However, the evidence does **not** establish that poor data quality is the root cause, that a dashboard would solve the problem, or that AI would improve forecasting.

Three areas require validation before solution selection:

1. the authoritative revenue recognition policy and owner;
2. the cause and measured effort of reconciliation;
3. the baseline forecast accuracy and variance process.

## POPIT-V Findings

### People

- Financial Control is reported as approving recognised revenue.
- Specialist interpretation appears concentrated in Finance roles.
- Policy ownership remains unknown.

### Organisation

- Finance and commercial teams appear to use revenue terminology differently.
- Ownership boundaries between commercial inputs, FP&A and Financial Control require further mapping.

### Process

- Forecasting includes commercial submissions plus Finance adjustments.
- Manual reconciliation occurs across multiple spreadsheets.
- Late commercial changes affect month-end forecast movement.

### Information

- "Revenue" is not consistently defined across teams.
- Commercial forecast, contract information and ledger postings reportedly use different identifiers.
- The authoritative recognition policy was not available.

### Technology

- Spreadsheets are part of the current reconciliation workflow.
- The workshop does not establish whether technology is the root cause.

### Value

- Finance leadership values earlier confidence.
- Candidate measures: forecast accuracy, reconciliation effort, variance explanation time.
- Baselines are currently unknown.

---

# Evidence Register

| ID | Evidence | Supports | Confidence |
|---|---|---|---|
| EVD-003 | FP&A Lead workshop statement on forecast preparation | PRC-001 / DEC-001 | Medium |
| EVD-004 | Revenue Accountant definition of recognised revenue | INF-002 / BR-001 | Medium |
| EVD-005 | Analyst statement on differing commercial use of "revenue" | INF-001 conflict | Medium |
| EVD-006 | Financial Controller statement on approval ownership | DEC-002 | Medium |
| EVD-007 | Analyst description of three-spreadsheet reconciliation | PAIN-001 | Medium |
| EVD-008 | Analyst estimate of two days reconciliation | VAL-002 hypothesis | Low |
| EVD-009 | Finance Director statement on earlier confidence | VAL-001 | Medium |
| EVD-010 | Group agreement on candidate measures | VAL-001 / VAL-002 / VAL-003 | Medium |

---

# Capability / Process Findings

| ID | Type | Name | Current Understanding | Evidence | Status |
|---|---|---|---|---|---|
| CAP-001 | Capability | Finance Planning & Control | Candidate capability encompassing the forecasting and recognition decisions explored in this simulation | EVD-003, EVD-004, EVD-006 | Unvalidated |
| PRC-001 | Process | Monthly Forecasting | Commercial submissions are incorporated and adjusted using Finance assumptions | EVD-003 | Unvalidated |
| PRC-002 | Process | Revenue Recognition | Finance determines which revenue can be recognised for the period and Financial Control is reported as the approval point | EVD-004, EVD-006 | Unvalidated |

These labels are working discovery constructs rather than claims about a real organisational capability model.

---

# Decision Catalogue

| ID | Decision | Owner | Trigger | Information | Rules | Action | Evidence | Status |
|---|---|---|---|---|---|---|---|---|
| DEC-001 | What revenue should be included in the current Finance forecast? | FP&A Lead (reported) | Forecast cycle / changes | INF-001, INF-003 | UNKNOWN | Update forecast | EVD-003 | Unvalidated |
| DEC-002 | What revenue can be recognised in the current period? | Financial Control (reported) | Month end / recognition event | INF-002, INF-004 | BR-001 | Approve / post recognised revenue | EVD-004, EVD-006 | Unvalidated |

---

# Information / Concept Findings

| ID | Concept / Requirement | Current Understanding | Status |
|---|---|---|---|
| INF-001 | Forecast Revenue | Commercial and Finance usage may differ | Conflicted |
| INF-002 | Recognised Revenue | Revenue meeting Finance recognition rules for the period | Unvalidated |
| INF-003 | Commercial Forecast Submission | Input into FP&A forecast | Unvalidated |
| INF-004 | Contractual / Delivery Condition Evidence | Required for recognition decision | Unvalidated |

---

# Business Rule Catalogue

| ID | Rule | Owner | Evidence | Status |
|---|---|---|---|---|
| BR-001 | Revenue cannot be recognised until relevant contractual and delivery conditions are met | UNKNOWN | EVD-004 | Unvalidated |

---

# Business Actions

| ID | Action | Triggered By | Evidence | Status |
|---|---|---|---|---|
| ACT-001 | Update the Finance forecast | DEC-001 | EVD-003 | Unvalidated |
| ACT-002 | Approve / post recognised revenue | DEC-002 | EVD-004, EVD-006 | Unvalidated |

---

# Pain Point Register

| ID | Pain Point | Impact | Evidence | Root Cause Status | Confidence |
|---|---|---|---|---|---|
| PAIN-001 | Manual reconciliation across three spreadsheets | Reported analyst effort and delay | EVD-007, EVD-008 | Unknown | Medium |
| PAIN-002 | Different meanings of "revenue" across teams | Risk of inconsistent interpretation | EVD-004, EVD-005 | Partially evidenced | Medium |
| PAIN-003 | Late commercial changes move the forecast near month end | Reduced earlier forecast confidence | Workshop statement | Unknown | Low |

---

# Assumptions and Open Questions

| ID | Type | Item | Status |
|---|---|---|---|
| ASM-001 | Assumption | A dashboard would materially improve the problem | Still unproven |
| ASM-002 | Assumption | AI would improve forecast accuracy | Still unproven |
| ASM-003 | Assumption | Poor source data quality is the root cause | Conflicted / unproven |
| OQ-001 | Open Question | Which decisions are being delayed or weakened? | Partially answered — DEC-001 and DEC-002 identified; impact needs validation |
| OQ-002 | Open Question | What does forecast revenue mean across the teams involved? | Conflict identified; definition unresolved |
| OQ-003 | Open Question | What is the authoritative recognition rule and who owns it? | Open |
| OQ-004 | Open Question | What specifically causes the reconciliation? | Open |
| OQ-005 | Open Question | What are the current baselines for success measures? | Open |

---

# Opportunity Register

| ID | Opportunity | Related Need | Expected Outcome | Evidence | Confidence |
|---|---|---|---|---|---|
| OPP-001 | Establish consistent Finance revenue definitions and ownership | PAIN-002 | More consistent interpretation and reporting | EVD-004, EVD-005 | Medium |
| OPP-002 | Reduce manual reconciliation by understanding identifier and information mismatches | PAIN-001 | Lower effort and faster month-end analysis | EVD-007 | Medium |
| OPP-003 | Improve visibility of forecast drivers and material variance | PAIN-003 / VAL-001 | Earlier confidence and faster explanation | EVD-009, EVD-010 | Low–Medium |

No technology solution has yet been selected for these opportunities.

---

# Benefits / Value Register

| ID | Value | Measure | Baseline | Evidence | Status |
|---|---|---|---|---|---|
| VAL-001 | Earlier confidence in revenue outlook | Point in month at which material forecast confidence is achieved | UNKNOWN | EVD-009 | Hypothesis |
| VAL-002 | Reduced reconciliation effort | Analyst hours/days per close | UNKNOWN | EVD-008 | Hypothesis |
| VAL-003 | Faster explanation of material variance | Time from variance detection to agreed explanation | UNKNOWN | EVD-010 | Hypothesis |

## Validation Priority

1. Obtain recognition policy and owner.
2. Observe / map reconciliation and quantify effort.
3. Calculate baseline forecast accuracy and variance behaviour.
4. Validate revenue definitions with commercial stakeholders.
