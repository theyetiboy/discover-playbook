---
title: "Process Modelling"
version: "1.2"
status: "Practitioner Technique"
---

# Process Modelling

> *"A process model is useful when it explains how work, decisions and information actually flow—not when it merely documents boxes and arrows."*

## Purpose

Process Modelling represents how work is performed from trigger to outcome, including activities, actors, information, decisions, controls, exceptions and hand-offs.

Within DISCOVER, process modelling is used to discover the business, not simply document an existing procedure.

## Why This Matters

Many apparent data or technology problems arise from:

- unclear process boundaries;
- re-keying;
- queues;
- duplicate approvals;
- poorly timed information;
- conflicting rules;
- exceptions;
- hand-offs between teams.

Process modelling creates a shared view that can be challenged and validated.

## What Process Modelling Is Not

It is not:

- a capability map;
- a system architecture;
- a project plan;
- a data lineage diagram;
- a list of standard operating procedures.

These artefacts can relate to one another but answer different questions.

## Levels of Modelling

Choose the appropriate level:

1. **Value Stream** — end-to-end value flow.
2. **Business Process** — major flow from trigger to business outcome.
3. **Sub-process** — focused detail.
4. **Procedure** — detailed instructions.

Start broad. Detail should be pulled by an important question, risk or decision.

## How It Fits DISCOVER

Useful during:

- Investigate;
- Study;
- Capture;
- Organise;
- Validate;
- Evaluate.

A process model often becomes the bridge to Decision, Information and Technology analysis.

## Core Elements

Capture as appropriate:

- trigger;
- outcome;
- actor / role;
- activity;
- decision;
- information input;
- information output;
- business rule;
- control;
- wait;
- exception;
- system;
- external party.

## Suggested Process

### 1. Define Boundaries

- What triggers the process?
- Where does it end?
- What outcome is created?
- What is out of scope?

### 2. Identify Actors

Map roles rather than only teams.

### 3. Map the Happy Path

Capture the major flow quickly.

### 4. Add Decisions and Information

For every decision ask:

- who decides;
- what information is required;
- what rule applies;
- what action follows.

### 5. Add Exceptions

Ask:

- What happens when the information is missing?
- What if the customer changes something?
- What if approval is rejected?
- What if the source system is late?
- What if the rule is ambiguous?

### 6. Add Controls and Waits

Make visible:

- approvals;
- reconciliation;
- segregation of duties;
- queues;
- waiting for data;
- waiting for specialists.

### 7. Validate the Model

Use people who actually perform the work.

## BPMN

BPMN 2.0.2 is useful where a formal process notation is needed. It provides standard concepts for events, activities, gateways, participants and message flows.

However, the goal is shared understanding. A simpler notation is often better in early workshops.

Use BPMN when:

- a formal model will be maintained;
- process automation is likely;
- several process variants must be compared;
- downstream architecture/design needs precision.

Do not make stakeholders learn BPMN before they can contribute.

## Discovery Questions

### Trigger / Outcome
- What starts this?
- What does “done” mean?
- Who receives the result?

### Activities
- What happens next?
- Which work is manual?
- Which work happens outside the main system?

### Decisions
- Where does judgement occur?
- Who decides?
- What information is needed?
- Which rule determines the path?

### Hand-offs
- Which team receives the work next?
- What format is transferred?
- What is commonly missing?
- How long does it wait?

### Exceptions
- What goes wrong?
- Which exception is most common?
- Which exception is most expensive or risky?
- Who can override?

### Controls
- Why does this step exist?
- What risk does it mitigate?
- How is the control evidenced?

## Finance Example

Model month-end close at the level needed to identify:

- upstream data receipt;
- reconciliation;
- journals;
- approvals;
- adjustments;
- consolidation;
- reporting;
- exceptions.

Do not begin by documenting every journal instruction. First find where Finance spends time and where decisions/rules matter.

## Marketing Example

Model a campaign from objective through planning, activation and measurement.

Important discovery points:

- audience selection;
- budget approval;
- channel choice;
- creative approval;
- tagging/measurement setup;
- optimisation decision;
- performance review.

## Outputs

- Process Map;
- BPMN model where appropriate;
- Decision Catalogue;
- Business Rules Catalogue;
- Information Flow;
- Control Register;
- Exception Catalogue;
- Pain Point Register;
- Golden Thread Traceability.

## Common Pitfalls

- mapping only the happy path;
- creating enormous diagrams;
- confusing capability with process;
- assuming documentation matches reality;
- designing the future state during current-state elicitation;
- ignoring information and decision flow;
- treating every delay as waste without understanding control/risk;
- inventing cycle times.

## Connection to Other Techniques

**Capability Mapping** tells you where to investigate.

**Process Modelling** shows how work flows.

**EventStorming** can rapidly discover events and hotspots.

**Value Stream Mapping** adds flow/time/value perspective.

**Decision Modelling** clarifies complex rules.

**Ontology Discovery** clarifies the concepts exchanged through the process.

## Practitioner Checklist

- [ ] Trigger and outcome are clear.
- [ ] Scope is proportionate.
- [ ] Actors are represented.
- [ ] Decisions are visible.
- [ ] Information is visible.
- [ ] Rules/controls are captured.
- [ ] Exceptions are represented.
- [ ] Model reflects reality.
- [ ] Pain points are evidenced.
- [ ] Model has been validated.

## References

- Object Management Group (OMG), *Business Process Model and Notation (BPMN) Version 2.0.2*.
- Object Management Group (OMG), *Decision Model and Notation (DMN) Version 1.5*.
- International Institute of Business Analysis (IIBA), *BABOK® Guide, Version 3*.
- Rummler, G. & Brache, A. (2012), *Improving Performance*, 3rd ed.

## Chapter Summary

Process Modelling helps DISCOVER move from broad capability understanding to the concrete flow of work, decisions and information. The model is a means to learn and validate, not an end in itself.
