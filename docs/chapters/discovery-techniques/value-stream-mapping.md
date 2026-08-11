---
title: "Value Stream Mapping"
version: "1.2"
status: "Practitioner Technique"
---

# Value Stream Mapping

> *"Optimising one activity is not the same as improving the flow of value."*

## Purpose

Value Stream Mapping (VSM) examines an end-to-end flow of work from demand or trigger to value, making visible:

- processing time;
- waiting;
- hand-offs;
- information flow;
- rework;
- bottlenecks;
- constraints.

Within DISCOVER it is adapted beyond manufacturing to business, data, analytical and knowledge-work contexts.

## Why This Matters

Teams often optimise their own step while the end-to-end outcome remains slow.

Examples:

- a Finance team automates a report but still waits days for upstream approval;
- Marketing improves dashboard refresh but campaign identifiers remain inconsistent;
- a data pipeline runs hourly while the source system updates weekly;
- a Rights team processes checks quickly but Sales waits for missing contract data.

VSM creates an end-to-end lens.

## Core Concepts

### Value
Value is defined by the business/customer outcome, not by whether a step is busy.

### Work Time
Time actively spent progressing the work.

### Wait Time
Time the work is not progressing.

### Lead / Cycle Time
Elapsed time through the value stream.

### Rework
Work repeated because of defects, missing information or changed decisions.

### Information Flow
How instructions, decisions, data and status move.

### Bottleneck
A constraint limiting overall flow.

## How It Fits DISCOVER

Use VSM during:

- Study;
- Capture;
- Organise;
- Evaluate.

It is especially useful when the complaint is:

- “it takes too long”;
- “there are too many hand-offs”;
- “we spend all our time reconciling”;
- “nobody knows where it is”;
- “we cannot scale”.

## When to Use It

Use when:

- the outcome crosses several teams;
- waiting is suspected to be significant;
- the process has repeated rework;
- manual data flow is important;
- local optimisation is likely;
- you need to quantify current-state friction.

## When Not to Use It

Do not force detailed timing when:

- timings are not available;
- the problem is primarily semantic;
- the scope is too broad to define one value stream;
- stakeholder confidence is still low.

Mark timing `UNKNOWN` rather than guessing.

## Suggested Approach

### 1. Define the Value

Ask:

- What outcome does the customer/business need?
- Who receives it?
- What makes the outcome valuable?

### 2. Set Boundaries

Define start and finish.

### 3. Map Major Stages

Capture major work stages rather than every task.

### 4. Add Information Flow

Show:

- requests;
- decisions;
- data;
- approvals;
- status;
- reports.

### 5. Add Time and Quality Evidence

Where evidence exists, capture:

- process time;
- wait time;
- queue;
- frequency;
- defect/rework;
- volume.

### 6. Identify Constraints

Look for:

- bottlenecks;
- repeated clarification;
- batch processing;
- late information;
- specialist dependency;
- approval delay;
- duplicate checks.

### 7. Design Improvement Hypotheses

Only after the current state is validated.

## Discovery Questions

- What is the customer/business outcome?
- How often is this value stream triggered?
- Where does work wait?
- What is the longest delay?
- Which queue is largest?
- What causes rework?
- Where is information missing?
- What is batched and why?
- Which step is constrained by specialist knowledge?
- Which work is performed “just in case”?
- Which control is mandatory?
- What happens when demand increases?

## Knowledge-Work Adaptation

In data/analytics discovery, VSM can map flows such as:

**Question → Data Request → Data Preparation → Analysis → Review → Insight → Decision**

or:

**Contract Event → Data Capture → Accounting Assessment → Recognition → Reconciliation → Report**

Focus on information and decision flow as much as task flow.

## Finance Example

A forecasting value stream might reveal:

- 2 hours preparing a file;
- 2 days waiting for commercial input;
- 1 day reconciling conflicting definitions;
- 30 minutes consolidating;
- 2 days waiting for approval.

The biggest opportunity may not be automation of consolidation.

## Marketing Example

A campaign insight value stream might expose:

- late agency cost data;
- inconsistent campaign identifiers;
- manual spreadsheet stitching;
- several review cycles;
- dashboards refreshed faster than decisions are made.

## Outputs

- Current-State Value Stream Map;
- validated time/quality measures;
- bottleneck register;
- Pain Point Register;
- Opportunity Register;
- Future-State hypotheses;
- Golden Thread links to value.

## Common Pitfalls

- inventing timings;
- mapping only process, not information;
- labelling every non-customer-facing activity waste;
- removing controls without understanding risk;
- focusing on one team rather than end-to-end flow;
- designing technology before root cause is understood.

## Practitioner Checklist

- [ ] Value recipient and outcome are defined.
- [ ] Boundaries are clear.
- [ ] Major stages are visible.
- [ ] Information flow is represented.
- [ ] Wait and rework are distinguished from work.
- [ ] Measures are evidence-based.
- [ ] Constraints are validated.
- [ ] Improvement hypotheses connect to value.

## References

- Rother, M. & Shook, J., *Learning to See*. Lean Enterprise Institute.
- Womack, J.P. & Jones, D.T. (2003), *Lean Thinking*, 2nd ed. Free Press.
- Lean Enterprise Institute, guidance on Value-Stream Mapping.

## Chapter Summary

Value Stream Mapping helps DISCOVER see the whole flow rather than optimise isolated activities. In data and knowledge work, the most important delays are often information, decisions and hand-offs.
