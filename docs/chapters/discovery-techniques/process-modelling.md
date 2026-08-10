---
title: "Process Modelling"
version: "1.0"
author: "Steve Tarry"
technique: "Discovery Technique"
---

# Process Modelling

## Purpose

Process Modelling is the practice of visually representing how work is performed within an organisation.

A process model can describe:

- What triggers work
- Which activities take place
- Who performs those activities
- What decisions are made
- What information is required
- Which systems are used
- Where handovers occur
- What outputs are created
- What exceptions can occur

The International Institute of Business Analysis (IIBA) describes process modelling as a standardised graphical model used to show how work is carried out and as a foundation for process analysis (IIBA, n.d.a).

Within DISCOVER, Process Modelling is used to understand both the **current state** and, where appropriate, the **future state** of a business process.

It is particularly useful during the **Investigate**, **Study**, **Capture**, **Validate** and **Evaluate** stages of DISCOVER.

---

# Why This Technique Matters

Business processes often evolve over many years.

As organisations change, processes can accumulate:

- Manual workarounds
- Duplicate activities
- Additional approvals
- Spreadsheet dependencies
- System handovers
- Reconciliations
- Exceptions
- Undocumented business rules

Individual stakeholders may understand their part of a process without understanding the complete end-to-end flow.

Process Modelling makes that flow visible.

It allows stakeholders to collectively examine:

```text
What happens?

Who does it?

Why does it happen?

What information is required?

Which system supports it?

Where does it go wrong?

What value does it create?
```

This shared understanding provides a stronger basis for identifying problems and designing improvements.

---

# When to Use Process Modelling

Process Modelling is particularly useful when:

- Understanding an unfamiliar business area
- A process involves multiple teams
- Responsibilities are unclear
- Significant manual work exists
- Spreadsheets are heavily used
- Information moves between systems
- Reconciliation is common
- Processes contain frequent exceptions
- Reporting depends upon operational processes
- Data quality problems need investigation
- Automation opportunities are being explored
- Data Products are being designed
- AI opportunities are being assessed
- A transformation programme is being planned

Process Modelling is especially useful when stakeholders describe a process differently.

The differences themselves are valuable discovery findings.

---

# What is a Business Process?

A Business Process is a sequence of activities performed to achieve a business outcome.

A process normally has:

```text
Trigger
   │
   ▼
Activities
   │
   ▼
Decisions
   │
   ▼
Outputs
   │
   ▼
Outcome
```

For example:

```text
Customer Order Received
        │
        ▼
Order Validated
        │
        ▼
Credit Checked
        │
        ▼
Order Approved
        │
        ▼
Product Delivered
        │
        ▼
Invoice Issued
        │
        ▼
Payment Received
```

The objective of discovery is to understand how the process actually operates rather than how documentation says it should operate.

---

# Process vs Capability

Capabilities and processes describe different perspectives of the business.

| Capability | Process |
|------------|---------|
| Describes what the organisation must be able to do | Describes how work is performed |
| Relatively stable | Changes more frequently |
| Outcome focused | Activity focused |
| Independent of a particular workflow | Describes a workflow |
| Useful for strategic planning | Useful for operational analysis |

For example:

```text
Capability

Revenue Management
```

may include processes such as:

```text
Revenue Forecasting

Revenue Recognition

Revenue Reconciliation

Revenue Reporting
```

One capability may therefore contain or depend upon several processes.

---

# Process Hierarchy

Processes can be represented at different levels of detail.

A simple DISCOVER hierarchy might use:

## Level 0 – Value Chain

The broadest view of how the organisation creates value.

Example:

```text
Create Content
    →
Sell Content
    →
Distribute Content
    →
Recognise Revenue
```

---

## Level 1 – End-to-End Process

A major business process.

Example:

```text
Order to Cash
```

---

## Level 2 – Process

A logical component of the end-to-end process.

Example:

```text
Contract Management

Billing

Revenue Recognition

Cash Collection
```

---

## Level 3 – Sub-Process

More detailed process behaviour.

Example:

```text
Validate Contract

Create Billing Schedule

Calculate Revenue

Post Revenue
```

---

## Level 4 – Activity / Task

Detailed operational activity.

Example:

```text
Download Contract Data

Validate Currency

Update Spreadsheet

Post Journal
```

The appropriate level depends upon the discovery objective.

Do not create detailed task-level maps when a high-level process view is sufficient.

---

# Current State and Future State

Process discovery frequently distinguishes between:

```text
AS-IS

How the process works today
```

and:

```text
TO-BE

How the process may work in the future
```

IIBA's Business Process Management perspective explicitly recognises modelling as a means of documenting and comparing current-state and future-state processes (IIBA, n.d.c).

DISCOVER normally starts with the current state.

Understanding the current process before designing the future process helps avoid:

- Automating unnecessary activity
- Replicating poor business rules
- Moving inefficient processes onto new technology
- Solving symptoms rather than causes

A useful principle is:

> **Understand the current reality before designing the future state.**

---

# Process Scope

Before modelling begins, establish the boundaries of the process.

Capture:

| Area | Question |
|------|----------|
| Trigger | What starts the process? |
| Start Point | Where does our scope begin? |
| End Point | Where does our scope end? |
| Outcome | What should the process achieve? |
| Customer | Who receives the outcome? |
| Owner | Who is accountable for the process? |
| Inputs | What information or materials are required? |
| Outputs | What does the process produce? |

Clear boundaries prevent workshops from expanding indefinitely.

---

# Process Trigger

Identify what starts the process.

Triggers might include:

```text
Customer Request Received

Contract Signed

Month End Reached

Campaign Approved

Programme Delivered

Invoice Received

Forecast Cycle Started
```

Ask:

- What causes the process to begin?
- Is the trigger scheduled or event driven?
- Who creates the trigger?
- Can several different triggers start the same process?

---

# Activities

Activities represent work performed during the process.

Use clear verb-based descriptions.

Examples:

```text
Validate Contract

Calculate Forecast

Approve Campaign

Create Invoice

Reconcile Revenue

Publish Report
```

Avoid vague labels such as:

```text
Processing

Admin

Review Stuff
```

The activity name should clearly describe what is happening.

---

# Decisions

Processes frequently contain decision points.

For example:

```text
Contract Valid?
      │
 ┌────┴────┐
 │         │
Yes        No
 │         │
 ▼         ▼
Continue   Return for Correction
```

Decision discovery is particularly valuable because decisions expose:

- Business rules
- Required information
- Ownership
- Exceptions
- Opportunities for analytics
- Opportunities for AI

Ask:

- What decision is being made?
- Who makes it?
- What information is required?
- What rule determines the outcome?
- Is the decision subjective?
- Are exceptions allowed?

---

# Roles and Responsibilities

Identify who performs each activity.

A simple swimlane model can show responsibility:

```text
Sales             Finance             Technology

  │                  │                    │
  ▼                  │                    │
Contract Signed      │                    │
  │                  │                    │
  └─────────────────►│                    │
                     ▼                    │
               Contract Reviewed         │
                     │                    │
                     ▼                    │
               Revenue Calculated        │
                     │                    │
                     └───────────────────►│
                                          ▼
                                    Data Processed
```

Swimlanes make handovers visible and help expose ownership problems.

---

# Handovers

Handovers occur where work or information moves between:

- People
- Teams
- Departments
- Systems
- Organisations

Handovers are important because they frequently introduce:

- Delay
- Miscommunication
- Data loss
- Duplicate entry
- Reconciliation
- Ownership ambiguity

Ask:

- What is handed over?
- Who sends it?
- Who receives it?
- How is it transferred?
- What happens if information is incomplete?
- How does the receiving team know it is ready?

---

# Information

Every process consumes and creates information.

For each activity ask:

```text
What information is needed?

Where does it come from?

Who owns it?

Can it be trusted?

What information is created?

Where does that information go next?
```

Examples include:

```text
Customer

Contract

Programme

Campaign

Rights

Forecast

Invoice

Revenue

Territory
```

These concepts should connect to:

- Business Glossary
- Ontology
- Data Catalogue
- KPI Catalogue

Process Modelling therefore provides an important bridge between business activity and data discovery.

---

# Systems

Once the business process is understood, identify the supporting technology.

For example:

```text
Activity                System

Create Opportunity      CRM

Create Contract         Contract Platform

Create Invoice          ERP

Calculate Forecast      Spreadsheet

Publish Report          BI Platform
```

This can reveal:

- Multiple systems supporting one process
- Duplicate functionality
- Manual data transfer
- Spreadsheet dependency
- Integration problems
- Legacy technology constraints

Avoid starting process discovery with the systems.

Start with the business activity, then identify how technology supports it.

---

# Business Rules

Business rules frequently sit behind activities and decisions.

Examples:

```text
Invoices above £X require additional approval.

Revenue may only be recognised when specified criteria are met.

Campaigns above a defined budget require executive approval.

A contract cannot become active until all mandatory information is complete.
```

Rules discovered during Process Modelling should be captured separately where they are important.

Ask:

- Why does this step occur?
- What rule determines the outcome?
- Is the rule documented?
- Who owns it?
- Does it vary?
- Are there exceptions?

---

# Exceptions

Do not model only the happy path.

Ask:

```text
What happens when this goes wrong?
```

Examples:

```text
Contract information missing

Invoice rejected

Campaign approval delayed

Revenue does not reconcile

System unavailable

Customer disputes payment
```

Exceptions often expose the real complexity of a business process.

They may also explain why stakeholders have created manual workarounds.

---

# Pain Points

Capture pain points directly against the process.

Examples:

```text
Manual data entry

Duplicate approval

Spreadsheet reconciliation

Long wait time

Missing information

Unclear ownership

Repeated rework

System limitation
```

A simple model might show:

```text
Contract Signed
      │
      ▼
Contract Entered
into Finance System
      │
      │  ⚠ Manual Re-keying
      ▼
Revenue Schedule
Created
      │
      │  ⚠ Spreadsheet
      ▼
Revenue
Recognised
```

This makes operational problems visible in context.

---

# Process Performance

Where possible, capture quantitative information.

Potential measures include:

- Process Volume
- Processing Time
- Waiting Time
- Cycle Time
- Failure Rate
- Rework Rate
- Error Rate
- Cost
- Automation Rate
- SLA Performance

For example:

| Measure | Current |
|---------|---------|
| Monthly Volume | 2,500 |
| Average Processing Time | 20 minutes |
| Average Waiting Time | 2 days |
| Rework Rate | 15% |
| Manual Processing | 70% |

Measurements should be validated rather than estimated where possible.

Process performance information can later support prioritisation and benefit measurement.

---

# Process Modelling Notations

Different levels of notation can be used depending upon the audience and purpose.

DISCOVER does not require every process to be documented using formal BPMN.

Possible approaches include:

- Simple Process Flow
- Swimlane Diagram
- SIPOC
- BPMN
- Value Stream Map
- Event Storming

The simplest notation capable of communicating the required information should normally be preferred during discovery.

---

# Simple Process Flow

A basic process flow may be sufficient for early discovery.

For example:

```text
Start
  │
  ▼
Receive Contract
  │
  ▼
Validate Contract
  │
  ▼
Contract Valid?
  │
 ┌┴────────────┐
 │             │
Yes            No
 │             │
 ▼             ▼
Create         Return for
Revenue        Correction
Schedule
 │
 ▼
End
```

The objective is shared understanding rather than diagramming sophistication.

---

# Swimlane Modelling

Swimlanes add responsibility to the process.

For example:

```text
Sales
────────────────────────────────────────
Create Contract
       │
       ▼

Finance
────────────────────────────────────────
Review Contract
       │
       ▼
Create Revenue Schedule
       │
       ▼

Reporting
────────────────────────────────────────
Publish Revenue
```

This is particularly useful when a process crosses organisational boundaries.

---

# BPMN

Business Process Model and Notation (BPMN) provides a standard graphical notation for representing business processes.

The Object Management Group (OMG) states that BPMN is intended to provide a standard notation that is understandable to business users while also being capable of representing complex process semantics for technical users (OMG, 2014).

BPMN 2.0.2 is also published internationally as ISO/IEC 19510:2013.

DISCOVER practitioners do not need to use every element of BPMN.

For many discovery situations, a small subset is sufficient.

---

# Useful BPMN Elements

## Start Event

Indicates where the process begins.

```text
○
```

---

## End Event

Indicates where the process finishes.

```text
●
```

---

## Activity / Task

Represents work being performed.

```text
┌─────────────────┐
│ Validate Invoice│
└─────────────────┘
```

---

## Sequence Flow

Shows the order of activities.

```text
Activity A
    │
    ▼
Activity B
```

---

## Gateway

Represents a decision or branching point.

```text
        ◇
      /   \
    Yes    No
```

---

## Pool / Lane

Shows responsibility.

For example:

```text
┌───────────────────────────────────────┐
│ Sales                                 │
├───────────────────────────────────────┤
│ Finance                               │
├───────────────────────────────────────┤
│ Technology                            │
└───────────────────────────────────────┘
```

These elements are normally sufficient for many high-level discovery models.

---

# Process Modelling Workshop

A DISCOVER Process Modelling workshop might follow this structure.

| Stage | Activity |
|-------|----------|
| 1 | Confirm purpose and scope |
| 2 | Define trigger and outcome |
| 3 | Identify high-level activities |
| 4 | Arrange activities in sequence |
| 5 | Identify roles and ownership |
| 6 | Identify decisions |
| 7 | Capture business rules |
| 8 | Identify information |
| 9 | Identify systems |
| 10 | Explore exceptions |
| 11 | Capture pain points |
| 12 | Capture opportunities |
| 13 | Validate the end-to-end model |

Do not attempt to make the diagram perfect during the conversation.

Capture the reality first.

Clean up the representation afterwards.

---

# Generic Discovery Questions

## Scope

- What process are we exploring?
- What triggers it?
- Where does it start?
- Where does it end?
- What outcome should it produce?
- Who owns the process?

---

## Activities

- What happens first?
- What happens next?
- Why does this activity happen?
- Is this activity always required?
- What happens immediately afterwards?

---

## People

- Who performs this activity?
- Who approves it?
- Who is accountable?
- Who needs to be consulted?
- Who needs to be informed?

---

## Decisions

- What decisions are made?
- Who makes them?
- What information is needed?
- Which rules determine the decision?
- What happens if the decision is rejected?

---

## Information

- What information is required?
- Where does it come from?
- Who owns it?
- Is it complete?
- Is it trusted?
- What information is created?

---

## Technology

- Which system supports this activity?
- Is any work performed outside the system?
- Are spreadsheets used?
- Is information copied manually?
- Are systems integrated?
- Is duplicate entry required?

---

## Handovers

- Where does responsibility change?
- What information is transferred?
- How is it transferred?
- Does the receiving team need to validate it?
- Where do delays occur?

---

## Exceptions

- What happens when something goes wrong?
- Which exceptions occur most frequently?
- What requires manual intervention?
- What causes rework?
- Who resolves exceptions?

---

## Performance

- How frequently does the process run?
- What volume does it handle?
- How long does it take?
- Where is most time spent?
- Where is most time lost?
- How frequently does rework occur?

---

## Improvement

- Which steps add little value?
- Which activities could be removed?
- Which activities could be simplified?
- Which tasks could be automated?
- Which decisions need better information?
- Where could Data Products help?
- Where could AI help?

---

# Process Discovery Through Observation

Stakeholder descriptions should not always be assumed to represent the complete process.

Where appropriate, observe the process directly.

This may reveal:

- Undocumented spreadsheets
- Copy-and-paste activity
- Personal notes
- Email approvals
- Manual calculations
- Unofficial workarounds
- Repeated system switching

A useful discovery question is:

> **Can you show me how you actually do this?**

The difference between documented process and actual behaviour can be one of the most valuable discovery findings.

---

# Process Walkthrough

A walkthrough allows a stakeholder to demonstrate a real example from beginning to end.

For example:

```text
"Show me the last contract you processed."
```

Then explore:

```text
Where did it arrive?

What did you do first?

What did you check?

What system did you open?

What information was missing?

Who did you contact?

What happened next?
```

Using a real example often produces richer information than asking stakeholders to describe the process abstractly.

---

# Current State Analysis

Once the current-state process is understood, assess it systematically.

Consider:

| Dimension | Questions |
|-----------|-----------|
| People | Are responsibilities clear? |
| Process | Are activities necessary and efficient? |
| Information | Is required information available and trusted? |
| Technology | Does technology support or constrain the process? |
| Control | Are appropriate controls present? |
| Performance | Is the process meeting expectations? |
| Value | Does each activity contribute to the required outcome? |

This analysis can produce a structured set of findings.

---

# Future State Design

Future-state design should be based upon identified problems and desired outcomes.

Possible changes might include:

```text
Remove Activity

Simplify Activity

Automate Activity

Change Ownership

Improve Information

Integrate Systems

Introduce Data Product

Introduce AI Assistance

Remove Duplicate Approval
```

The future-state process should explicitly show how these changes address identified problems.

Avoid redesigning the process simply to introduce new technology.

---

# Process Improvement Opportunities

Process discovery may reveal several categories of opportunity.

## Eliminate

Remove unnecessary activity.

Example:

```text
Duplicate approval no longer required.
```

---

## Simplify

Reduce complexity.

Example:

```text
Replace multiple templates with one standard submission.
```

---

## Standardise

Create consistent ways of working.

Example:

```text
Use one recognised revenue definition across reporting.
```

---

## Integrate

Improve information movement.

Example:

```text
Transfer approved contract information automatically to Finance.
```

---

## Automate

Automate predictable activities.

Example:

```text
Automatically reconcile matching transactions.
```

---

## Inform

Improve decision-making through better data.

Example:

```text
Provide real-time forecast variance information.
```

---

## Augment

Use AI to support human activity.

Example:

```text
Summarise complex contracts for Finance review.
```

The appropriate response depends upon the cause of the problem.

---

# Connecting Process Modelling to POPIT-V

Process Modelling is naturally centred on the **Process** dimension of POPIT-V, but effective analysis requires all six perspectives.

## People

- Who performs the work?
- Who makes decisions?
- Where is specialist knowledge concentrated?

## Organisation

- Who owns the process?
- Which teams participate?
- Where do governance boundaries exist?

## Process

- What happens?
- In what order?
- Where are handovers, exceptions and delays?

## Information

- What information is required?
- What information is created?
- Which business rules apply?

## Technology

- Which systems support the process?
- Where are integrations missing?
- Where does manual work compensate for technology?

## Value

- What business outcome does the process create?
- Which activities add value?
- What would improvement deliver?

---

# Connecting Process Modelling to Capability Mapping

Business capabilities describe what the organisation needs to be able to do.

Processes describe how those capabilities are realised.

For example:

```text
CAPABILITY

Revenue Management
        │
        ├── Revenue Forecasting Process
        ├── Revenue Recognition Process
        ├── Revenue Reconciliation Process
        └── Revenue Reporting Process
```

This relationship creates traceability between strategy and operational activity.

---

# Connecting Process Modelling to Event Storming

Event Storming and Process Modelling are complementary techniques.

Event Storming is highly effective for collaborative exploration.

Process Modelling provides a more structured representation of the resulting workflow.

A useful pattern is:

```text
Event Storming
      │
      ▼
Discover What Happens
      │
      ▼
Identify Events,
Rules & Exceptions
      │
      ▼
Process Modelling
      │
      ▼
Document & Analyse
the Agreed Flow
```

Event Storming does not always need to precede Process Modelling.

The appropriate technique depends upon the complexity of the problem and the stakeholders involved.

---

# Connecting Process Modelling to the Business Glossary

Processes expose terminology.

For example:

```text
Validate Contract
        │
        ▼
Recognise Revenue
        │
        ▼
Calculate Royalty
```

Immediately raises concepts such as:

```text
Contract

Revenue

Royalty
```

These should be captured in the Business Glossary.

The process then provides useful context for understanding what those concepts mean and where they are used.

---

# Connecting Process Modelling to Ontology Discovery

Processes reveal relationships between concepts.

For example:

```text
Customer
    SIGNS
Contract

Contract
    GRANTS
Rights

Rights
    APPLY TO
Programme
```

Process discovery also reveals lifecycle events such as:

```text
Contract Created

Contract Approved

Contract Signed

Contract Expired
```

These concepts, relationships and lifecycle states can feed directly into ontology development.

---

# Connecting Process Modelling to Data Products

Processes identify where information is needed to support decisions.

For example:

```text
Revenue Review
      │
      ▼
Decision:
Are we on forecast?
```

The decision may require:

```text
Actual Revenue

Forecast Revenue

Contract Value

Territory

Currency

Variance
```

This may lead to a:

```text
Revenue Performance Data Product
```

A useful discovery pattern is therefore:

```text
Process
   │
   ▼
Decision
   │
   ▼
Information Required
   │
   ▼
Data Product
```

This reinforces a core DISCOVER principle:

> **Decisions drive data requirements.**

---

# Connecting Process Modelling to AI

Processes are a particularly useful way to discover potential AI opportunities.

Consider activities involving:

- Reading
- Searching
- Summarising
- Classifying
- Predicting
- Recommending
- Generating
- Reconciling
- Monitoring
- Decision support

For example:

```text
Contract Received
      │
      ▼
Contract Reviewed
      │
      ▼
Rights Identified
```

may reveal opportunities for:

```text
Document Classification

Contract Summarisation

Metadata Extraction

Rights Extraction
```

Another process:

```text
Actuals Received
      │
      ▼
Variance Analysed
      │
      ▼
Commentary Created
```

may reveal:

```text
Anomaly Detection

Variance Explanation

Automated Commentary
```

AI should not automatically be introduced simply because an activity could theoretically be automated.

The opportunity must still be evaluated against:

- Business value
- Data readiness
- Risk
- Accuracy requirements
- Human oversight
- Technology feasibility

using the DISCOVER AI Opportunity Canvas.

---

# Finance Example

## Discovery Objective

Understand the end-to-end monthly financial reporting process, including information flows, business rules, manual interventions and opportunities for improvement.

An initial process might be:

```text
Month End
Reached
   │
   ▼
Actuals
Received
   │
   ▼
Transactions
Validated
   │
   ▼
Revenue
Reconciled
   │
   ▼
Adjustments
Posted
   │
   ▼
P&L
Prepared
   │
   ▼
Variance
Analysed
   │
   ▼
Commentary
Created
   │
   ▼
Management
Report Published
```

### Example Questions

- What triggers the month-end process?
- Which teams contribute?
- When are source systems closed?
- Where do actuals originate?
- What reconciliations are performed?
- Which adjustments are manual?
- Who approves journals?
- How are exchange rates applied?
- How is forecast compared with actual?
- Who creates commentary?
- Which spreadsheets are used?
- Which steps create the greatest delay?
- What happens when figures do not reconcile?
- Which reports depend upon the process?

### Potential Pain Points

Discovery might reveal:

```text
Actuals arrive at different times.

Multiple spreadsheets are reconciled manually.

Revenue definitions vary between reports.

Currency conversion requires manual adjustment.

Commentary is created manually every month.

Data ownership is unclear.

Late changes cause repeated report regeneration.
```

### Potential Opportunities

These findings could lead to:

- Finance Data Product
- Revenue Performance Data Product
- Automated Reconciliation
- Standardised Finance Semantic Layer
- Forecast Variance Monitoring
- Automated Financial Commentary
- Finance Knowledge Assistant

---

# Marketing Example

## Discovery Objective

Understand the end-to-end campaign process from planning through to performance evaluation.

A simplified process might be:

```text
Campaign Need
Identified
   │
   ▼
Campaign Brief
Created
   │
   ▼
Budget
Approved
   │
   ▼
Audience
Selected
   │
   ▼
Creative
Produced
   │
   ▼
Campaign
Launched
   │
   ▼
Performance
Monitored
   │
   ▼
Campaign
Completed
   │
   ▼
Results
Analysed
   │
   ▼
Learning
Captured
```

### Example Questions

- What triggers a campaign?
- Who owns the campaign brief?
- How is budget approved?
- How are audiences selected?
- Which systems are used for activation?
- How are campaign identifiers created?
- Where is spend captured?
- How is performance measured?
- When is optimisation performed?
- How is attribution calculated?
- How is campaign ROI determined?
- Where is learning from previous campaigns stored?

### Potential Pain Points

Discovery may reveal:

```text
Campaign information exists across several systems.

Campaign identifiers are inconsistent.

Performance reporting is manually consolidated.

Audience definitions differ by platform.

Attribution models vary.

Historical campaign learning is difficult to retrieve.
```

### Potential Opportunities

These findings could lead to:

- Campaign Performance Data Product
- Marketing Semantic Layer
- Audience Data Product
- Campaign Taxonomy
- Automated Campaign Reporting
- Campaign Optimisation Models
- AI Campaign Insight Assistant

---

# Common Pitfalls

## Modelling the Documented Process Rather Than Reality

Documentation may describe what should happen.

Discovery needs to understand what actually happens.

Validate the model with people who perform the work.

---

## Starting With Technology

Do not begin with:

```text
Salesforce sends a file to Oracle.
```

Begin with:

```text
Contract Approved
        │
        ▼
Invoice Created
```

Then determine which systems support those activities.

---

## Going Into Too Much Detail

A process map containing hundreds of activities is difficult to understand.

Start high level.

Decompose only where further detail supports the discovery objective.

---

## Ignoring Exceptions

The happy path often represents only part of the work.

Exceptions may account for disproportionate effort and complexity.

---

## Mixing Current and Future State

Clearly distinguish:

```text
AS-IS
```

from:

```text
TO-BE
```

Otherwise stakeholders may lose confidence in the model.

---

## Designing Solutions Too Early

When a pain point appears, capture it.

Do not immediately redesign the entire process.

Complete enough discovery to understand the cause.

---

## Automating a Bad Process

Automation does not automatically improve a process.

First ask whether the activity:

- Needs to exist
- Can be simplified
- Can be standardised
- Can be removed

Only then consider automation.

---

## Creating Diagrams Nobody Can Read

Process models exist to communicate.

Use the level of notation appropriate for the audience.

Complex notation that stakeholders cannot understand reduces the value of the model.

---

# What Good Looks Like

An effective Process Model should:

- Have clear scope
- Identify the process trigger
- Identify the expected outcome
- Show major activities
- Show responsibility
- Show important decisions
- Capture key business rules
- Identify required information
- Identify supporting systems
- Show important handovers
- Include relevant exceptions
- Capture pain points
- Identify opportunities
- Be validated by stakeholders
- Be understandable by its intended audience

Most importantly, the model should help the organisation understand **how work really happens**.

---

# Discovery Outputs

Process Modelling should contribute to:

- Current-State Process Map
- Future-State Process Map
- Process Catalogue
- Process Ownership
- RACI Matrix
- Business Rules Catalogue
- Information Requirements
- System Dependencies
- Pain Point Register
- Opportunity Register
- Data Product Opportunities
- AI Opportunities
- KPI Requirements
- Roadmap

---

# Related DISCOVER Techniques

Process Modelling works particularly well alongside:

- Business Capability Mapping
- Business Glossary
- Domain-Driven Design
- Event Storming
- Ontology Discovery
- Stakeholder Mapping
- Value Stream Mapping
- Root Cause Analysis

A common discovery progression might be:

```text
Business Capability
        │
        ▼
Process Discovery
        │
        ▼
Event Storming / Walkthrough
        │
        ▼
Current-State Process
        │
        ├──────────────► Business Rules
        ├──────────────► Information
        ├──────────────► Systems
        ├──────────────► Pain Points
        └──────────────► Decisions
                              │
                              ▼
                         Opportunities
                              │
                    ┌─────────┴─────────┐
                    ▼                   ▼
               Data Products           AI
```

The exact sequence should depend upon the needs of the engagement.

---

# Recommended Discovery Questions – Quick Reference

Before concluding Process Modelling, ensure you can answer:

- What triggers the process?
- Where does it begin and end?
- What outcome does it produce?
- Who owns it?
- What are the major activities?
- Who performs each activity?
- What decisions are made?
- What information is required?
- Which business rules apply?
- Which systems are used?
- Where are the handovers?
- What exceptions occur?
- Where does rework occur?
- Where are the delays?
- Which activities are manual?
- Which spreadsheets are involved?
- What measures indicate performance?
- Which activities add little value?
- Where could the process be simplified?
- Where could better information improve decisions?
- Which Data Products could help?
- Where could AI or automation add value?
- What requires further investigation?

---

# References

International Institute of Business Analysis (IIBA) (n.d.a) *10.35 Process Modelling*. A Guide to the Business Analysis Body of Knowledge (BABOK® Guide). Available at: https://www.iiba.org/knowledgehub/business-analysis-body-of-knowledge-babok-guide/10-techniques/10-35-process-modelling/ (Accessed: 10 August 2026).

International Institute of Business Analysis (IIBA) (n.d.b) *10.34 Process Analysis*. A Guide to the Business Analysis Body of Knowledge (BABOK® Guide). Available at: https://www.iiba.org/knowledgehub/business-analysis-body-of-knowledge-babok-guide/10-techniques/10-34-process-analysis/ (Accessed: 10 August 2026).

International Institute of Business Analysis (IIBA) (n.d.c) *11.5 The Business Process Management Perspective*. A Guide to the Business Analysis Body of Knowledge (BABOK® Guide). Available at: https://www.iiba.org/knowledgehub/business-analysis-body-of-knowledge-babok-guide/11-perspectives/11-5-the-business-process-management-perspective/ (Accessed: 10 August 2026).

International Organization for Standardization (ISO) (2010) *ISO 10244:2010 Document management — Business process baselining and analysis*. Geneva: International Organization for Standardization. Available at: https://www.iso.org/standard/45935.html (Accessed: 10 August 2026).

International Organization for Standardization (ISO) and International Electrotechnical Commission (IEC) (2013) *ISO/IEC 19510:2013 Information technology — Object Management Group Business Process Model and Notation*. Geneva: ISO.

Object Management Group (OMG) (2014) *Business Process Model and Notation (BPMN), Version 2.0.2*. Object Management Group. Available at: https://www.omg.org/spec/BPMN/2.0.2/ (Accessed: 10 August 2026).