---
title: "Process"
chapter: 13
version: "1.2"
status: "Practitioner Reference"
---

# Process

> *"Map what really happens—including exceptions and workarounds—not only the documented happy path."*

## Purpose

The **Process** perspective focuses on how work moves from a trigger to an outcome.

It seeks to understand activities, decisions, hand-offs, waits, controls, exceptions, rework, information dependencies and measures of performance.

Process discovery is not primarily about producing a beautiful diagram. Its purpose is to reveal how the business operates, where decisions occur, where information is required and where friction prevents value from flowing.

## Why This Matters

A report request may be caused by a process that creates information too late. A data quality problem may be caused by re-keying. A system complaint may actually be an approval bottleneck. A manual reconciliation may be compensating for two teams applying different business rules.

Without understanding process, teams can automate waste rather than remove it.

## Discovery Objectives

Understand:

- process purpose and outcome;
- trigger and completion state;
- actors and roles;
- major activities;
- inputs and outputs;
- business decisions;
- hand-offs;
- controls;
- exceptions;
- queues and waits;
- rework and reconciliation;
- manual interventions;
- dependencies;
- measures such as cycle time, quality and failure demand.

## What Good Looks Like

You should be able to answer:

- What triggers the work?
- What outcome indicates completion?
- What are the major steps?
- Who performs them?
- Where are the decisions?
- What information is needed at each decision?
- Which business rules affect routing or calculation?
- Where does work wait?
- Where are errors discovered?
- What happens in exceptions?
- Where is information re-keyed, exported or reconciled?
- Which controls are mandatory?
- How is process performance measured?

## Process Levels

Use the level of detail appropriate to the question.

### Value Stream / End-to-End Flow
A high-level view across organisational boundaries from demand to value.

### Business Process
A coherent sequence of activities producing a business outcome.

### Sub-process
A detailed portion of a wider process.

### Procedure / Work Instruction
The detailed steps for an individual task.

DISCOVER usually starts high enough to see the end-to-end outcome, then deepens only where evidence or risk justifies it.

## What to Discover

### Trigger and Outcome

Capture:

- triggering event;
- preconditions;
- intended customer/business outcome;
- completion criteria;
- downstream consequences.

### Activities

Understand:

- sequence;
- parallel work;
- batch activity;
- manual steps;
- automated steps;
- repeated tasks;
- non-value work.

### Decisions

For each material decision:

- decision owner;
- trigger;
- alternatives;
- information required;
- business rules;
- action produced;
- exception handling.

### Information Flow

Identify:

- information created;
- information consumed;
- documents;
- spreadsheets;
- reports;
- data entered;
- data transferred;
- information returned for correction.

### Hand-offs and Waits

Explore:

- team-to-team transfer;
- approvals;
- queues;
- dependency on specialists;
- SLA / service expectations;
- waiting for data;
- waiting for customer or supplier response.

### Controls

Understand:

- approvals;
- segregation of duties;
- reconciliations;
- validation;
- audit evidence;
- regulatory control;
- security and privacy checks.

Do not remove a step merely because it appears inefficient; first understand why it exists.

### Exceptions

Explore:

- common exceptions;
- rare but high-impact exceptions;
- manual overrides;
- escalation;
- rework;
- backdating;
- late changes;
- incomplete information.

### Measures

Potential measures:

- cycle time;
- wait time;
- throughput;
- first-time-right rate;
- exception rate;
- rework;
- SLA attainment;
- cost;
- quality;
- customer/business outcome.

## Generic Discovery Questions

### Scope

- What starts the process?
- What counts as complete?
- Who is the customer or beneficiary?
- What outcome is the process meant to create?

### Flow

- What happens first?
- What happens next?
- Which activities occur in parallel?
- Where does work leave one team and enter another?
- What is the longest wait?
- Where does the process loop back?

### Decisions

- Where does judgement occur?
- Who makes the decision?
- What information is used?
- Which rule determines the result?
- What happens when the decision is uncertain?

### Controls

- Why does this approval exist?
- What risk does it control?
- What evidence must be retained?
- What can be automated and what requires human judgement?

### Exceptions

- What breaks the happy path?
- Which exception occurs most often?
- Which exception causes the greatest risk?
- Who can override the normal process?
- How are late changes handled?

### Information

- What information is created at each step?
- Where is it re-keyed?
- Where are files downloaded or uploaded?
- Where are spreadsheets used?
- Which information is often missing or wrong?

### Performance

- How long does the process take?
- Which part is actual work versus waiting?
- How often is work returned?
- How is quality measured?
- What does a good outcome look like?


## Evidence to Capture

Do not treat workshop conversation as automatically validated fact. Capture important findings using the DISCOVER evidence model:

- **Evidence** — explicitly supported by a trusted source, observed artefact or validated record.
- **Stakeholder Statement** — stated by a stakeholder but not yet independently validated.
- **Assumption** — plausible but unverified.
- **Interpretation** — an analytical conclusion drawn from evidence.
- **Recommendation** — a proposed intervention.
- **Open Question** — information still required.

Where evidence conflicts, record the contradiction and identify who or what can validate it. Use `UNKNOWN` when an important Golden Thread link is not established.


## Modelling Notation

Use notation that stakeholders can understand.

For formal process models, BPMN 2.0.2 provides a widely adopted notation. However, early discovery may be better served by simple flows, sticky notes, EventStorming or value-stream views.

The model is valuable only if it improves shared understanding.

## Discovery Artefacts

- Process Map;
- Value Stream Map;
- Decision Catalogue;
- Business Rules Catalogue;
- Information Flow Diagram;
- Pain Point Register;
- Risk / Control Register;
- Evidence Register;
- Golden Thread Traceability.

## Typical Pain Points

- manual hand-offs;
- duplicate entry;
- spreadsheet dependency;
- long waits;
- excessive approvals;
- reconciliation;
- unclear exception handling;
- inconsistent process variants;
- poor visibility;
- hidden work;
- local workarounds;
- controls implemented differently by team;
- poor upstream information creating downstream rework.

## Opportunities

- simplify flow;
- remove duplicate activity;
- improve information at the point of decision;
- automate repeatable tasks;
- redesign approval thresholds;
- prevent errors upstream;
- standardise high-value rules;
- improve exception management;
- make status visible;
- reduce re-keying;
- create reusable process/data services;
- redesign the process before introducing AI.

## Maturity Signals

### Fragmented
Processes depend on individual knowledge, variants are uncontrolled, exceptions dominate and measurement is weak.

### Developing
Core flows are known but documentation and controls vary; workarounds remain common.

### Defined
Major processes, decisions, controls and owners are documented and validated.

### Managed
Performance is measured end-to-end, root causes are analysed and improvement is systematic.

### Adaptive
Processes evolve using evidence, automation and decision support while maintaining clear controls and value measures.

## Finance Example

### Revenue Recognition

Map from commercial event or contract milestone through accounting assessment, calculation, journal, reconciliation, approval and reporting.

Probe:

- what business event triggers recognition;
- which contract terms matter;
- who applies judgement;
- which rules and exceptions exist;
- how data moves from commercial/rights systems to Finance;
- where adjustments are manual;
- how recognised revenue is reconciled;
- what evidence supports audit.

### Forecasting

Map from assumptions and opportunity inputs through forecast preparation, challenge, adjustment, approval, consolidation and variance review.

Focus on **decision flow and information flow**, not just the spreadsheet mechanics.

## Marketing Example

Map the campaign lifecycle:

Objective → audience → budget → plan → creative/media → activation → measurement → optimisation → learning.

Identify separate decisions for planning, in-flight optimisation and post-campaign evaluation.


## Golden Thread Connection

This perspective should not exist as an isolated checklist. Connect findings to the Golden Thread wherever the evidence supports it:

**Business Strategy → Business Capability → Business Process → Business Decision → Business Information → Business Rules → Technology / Data → Data Product / Analytics → Insight / Action → Business Value**

Use stable identifiers when the engagement requires traceability:

- `STR-` Strategic Objective
- `CAP-` Business Capability
- `PRC-` Business Process
- `DEC-` Business Decision
- `INF-` Information
- `BR-` Business Rule
- `SYS-` System / Technology
- `DAT-` Data Asset
- `DP-` Data Product
- `ACT-` Business Action
- `VAL-` Business Value

Supporting discovery records may use `EVD-`, `ASM-`, `OQ-`, `PAIN-`, `OPP-` and `RSK-`.

The objective is traceability rather than bureaucracy. Do not invent links merely to complete the chain.


## Facilitation Cautions

- Map the current reality before designing the future.
- Include exceptions; they often explain the real cost.
- Do not over-model low-value detail.
- Ask “why does this step exist?” before removing it.
- Distinguish process from capability.
- Keep decision and information dependencies visible.
- Never invent timings; mark them unknown until measured.

## Practitioner Checklist

- [ ] Trigger and outcome are clear.
- [ ] Scope and level of detail are appropriate.
- [ ] Real actors are represented.
- [ ] Decisions and rules are visible.
- [ ] Information inputs/outputs are understood.
- [ ] Hand-offs, waits and exceptions are captured.
- [ ] Controls are understood before being challenged.
- [ ] Pain points are evidence-based.
- [ ] Process measures connect to value.
- [ ] Broken Golden Thread links are visible.

## References

- Object Management Group (OMG), *Business Process Model and Notation (BPMN) Version 2.0.2*.
- Object Management Group (OMG), *Decision Model and Notation (DMN) Version 1.5*.
- International Institute of Business Analysis (IIBA), *BABOK® Guide, Version 3*.
- Rother, M. & Shook, J., *Learning to See*. Lean Enterprise Institute.
- Rummler, G. & Brache, A. (2012), *Improving Performance*, 3rd ed. Jossey-Bass.

## Chapter Summary

The Process perspective reveals how work, decisions and information flow across the organisation. It enables DISCOVER to find bottlenecks, controls, exceptions and root causes before recommending automation, data products or AI.
