---
title: "Value Stream Mapping"
version: "1.0"
author: "Steve Tarry"
technique: "Discovery Technique"
---

# Value Stream Mapping

## Purpose

Value Stream Mapping (VSM) is a technique for understanding the end-to-end flow of activities and information required to deliver value to a customer or other beneficiary.

Rather than analysing individual process steps in isolation, Value Stream Mapping examines how work moves across the complete system.

The International Institute of Business Analysis (IIBA) describes Value Stream Mapping as a complete, fact-based and time-series representation of the activities required to deliver a product or service (IIBA, n.d.a).

Lean Enterprise Institute describes a value stream as the actions required to bring a product or service through the flow to the customer, including both value-creating and non-value-creating activity (Lean Enterprise Institute, n.d.a).

Within DISCOVER, Value Stream Mapping helps practitioners understand:

- How value flows through the organisation
- Where value is created
- Where work waits
- Where handovers occur
- Where information is delayed
- Where unnecessary effort exists
- Where bottlenecks constrain performance
- Where process improvement may create value
- Where Data Products could improve decisions
- Where automation or AI could improve flow

Value Stream Mapping is particularly useful during the **Study**, **Capture**, **Evaluate** and **Roadmap** stages of DISCOVER.

---

# Why This Technique Matters

Organisations are usually structured into functions.

For example:

```text
Sales

Legal

Rights

Finance

Operations

Technology

Data
```

Customers, however, rarely experience those organisational boundaries.

They experience an end-to-end outcome.

For example:

```text
Customer Request
       │
       ▼
Opportunity
       │
       ▼
Contract
       │
       ▼
Rights Confirmation
       │
       ▼
Delivery
       │
       ▼
Billing
       │
       ▼
Payment
```

Each department may optimise its own part of this flow while the overall customer journey remains slow or inefficient.

Value Stream Mapping encourages a **system-level view**.

Instead of asking:

> How efficient is Finance?

or:

> How efficient is Sales?

ask:

> How efficiently does value flow from the original need through to the final business outcome?

This distinction helps prevent local optimisation from being mistaken for end-to-end improvement.

---

# What is a Value Stream?

A Value Stream represents the sequence of activities required to deliver a product, service or outcome to a customer or beneficiary.

A simple example might be:

```text
Customer Need
      │
      ▼
Request Received
      │
      ▼
Request Evaluated
      │
      ▼
Proposal Created
      │
      ▼
Agreement Reached
      │
      ▼
Service Delivered
      │
      ▼
Customer Receives Value
```

The stream includes more than the visible process activities.

It can also include:

- Information flows
- Decisions
- Waiting
- Queues
- Approvals
- Rework
- Handoffs
- Systems
- Delays

Understanding these elements provides a more complete picture of how value is delivered.

---

# Start With Value

Value Stream Mapping should begin by understanding **who receives value and what outcome they require**.

Ask:

```text
Who is the customer?

What are they trying to achieve?

What outcome do they value?

What does success look like?

What makes the outcome timely, useful or high quality?
```

The customer may be external.

For example:

```text
Broadcaster

Distributor

Advertiser

Consumer

Licensee
```

The customer may also be internal.

For example:

```text
Finance Director

Sales Team

Marketing Team

Executive Leadership

Production Team
```

DISCOVER therefore uses the term **customer or beneficiary** broadly.

---

# Value From the Customer Perspective

Lean thinking places particular emphasis on defining value from the perspective of the customer.

This is important because an organisation may perform activities that make sense internally but do not improve the outcome delivered to the customer.

For each activity ask:

```text
Does this activity move us closer to the required outcome?

Would the customer notice if this activity disappeared?

Does this activity improve quality, timeliness or usefulness?

Is this activity necessary because of regulation, governance or control?

Is it simply the result of the way we currently operate?
```

These questions help distinguish different forms of activity.

---

# Value-Adding Activity

A Value-Adding activity directly contributes towards the required customer outcome.

Examples might include:

```text
Producing the requested analysis

Creating the programme

Delivering licensed content

Resolving the customer's request

Producing an approved campaign asset
```

Whether an activity adds value depends upon the value stream and customer.

---

# Necessary Non-Value-Adding Activity

Some activities may not directly create customer value but remain necessary.

Examples might include:

```text
Regulatory Control

Financial Control

Security Validation

Legal Review

Mandatory Audit

Compliance Check
```

The objective should not automatically be to remove these activities.

Instead ask:

> Can the required control be achieved more efficiently?

---

# Waste

Other activities may consume time or resources without creating necessary value.

Examples might include:

```text
Waiting

Duplicate Entry

Unnecessary Approval

Repeated Reconciliation

Searching for Information

Correcting Errors

Producing Unused Reports

Moving Information Between Spreadsheets
```

These are potential improvement opportunities.

They should be validated rather than assumed.

---

# Value Stream vs Process

Value Stream Mapping and Process Modelling are closely related but operate at different levels.

| Value Stream Mapping | Process Modelling |
|----------------------|------------------|
| Focuses on end-to-end value | Focuses on how a process operates |
| Looks across organisational boundaries | May focus on one process |
| Emphasises flow | Emphasises activities and decisions |
| Highlights waiting and queues | Highlights workflow |
| Includes information flow | May include information |
| Measures lead time | Often measures process behaviour |
| Supports system-level improvement | Supports detailed process improvement |

Lean Enterprise Institute distinguishes Value Stream Mapping as a way of understanding and improving the overall flow rather than optimising isolated process steps (Lean Enterprise Institute, 2022).

A useful DISCOVER relationship is:

```text
Value Stream
     │
     ├── Process A
     ├── Process B
     ├── Process C
     └── Process D
```

A Value Stream can therefore contain several processes.

---

# Value Stream vs Business Capability

These techniques also provide different perspectives.

```text
Business Capability

What must the organisation
be able to do?

          │

          ▼

Value Stream

How does value flow across
those capabilities?

          │

          ▼

Process

How is a particular part
of the work performed?
```

For example:

```text
VALUE STREAM

Licence Content to Customer
        │
        ├── Sales Management
        ├── Contract Management
        ├── Rights Management
        ├── Content Delivery
        ├── Billing
        └── Revenue Management
```

The value stream crosses multiple capabilities to produce one end-to-end outcome.

---

# Current-State Value Stream

Value Stream Mapping normally begins with the **current state**.

The purpose is to understand what actually happens today.

Lean Enterprise Institute describes current-state mapping as capturing the actual condition of the flow before designing a future-state map (Lean Enterprise Institute, n.d.a).

A simple current-state example might be:

```text
Customer
Request
  │
  ▼
Request
Reviewed
  │
  │
  │  2 Days Waiting
  ▼
Proposal
Prepared
  │
  │
  │  4 Days Waiting
  ▼
Legal
Review
  │
  │
  │  3 Days Waiting
  ▼
Agreement
Approved
  │
  ▼
Customer
Receives Outcome
```

The process activities themselves may only require several hours.

The end-to-end lead time may be several days or weeks.

This difference is extremely important.

---

# Future-State Value Stream

Once the current state is understood, a future-state map can describe a more effective flow.

For example:

```text
CURRENT STATE

Request
  │
  ▼
Review
  │
  │ 2 Days
  ▼
Prepare
  │
  │ 4 Days
  ▼
Approve
  │
  │ 3 Days
  ▼
Deliver


FUTURE STATE

Request
  │
  ▼
Automated Validation
  │
  ▼
Prepare
  │
  ▼
Risk-Based Approval
  │
  ▼
Deliver
```

The purpose of the future state is not simply to draw a cleaner diagram.

It should describe a realistic target state that addresses the problems exposed by current-state discovery.

Rother and Shook's Value Stream Mapping approach similarly progresses from current-state mapping to future-state design and then to an implementation plan (Rother and Shook, 1999).

---

# Current State Before Future State

Do not begin Value Stream Mapping by asking:

> What technology should we implement?

First understand:

```text
What is happening?

Where does value flow?

Where does work stop?

Why does it stop?

What information is missing?

Where does rework occur?

Why are controls required?
```

Otherwise there is a risk of automating waste rather than removing it.

---

# End-to-End Flow

The power of Value Stream Mapping comes from looking beyond individual departments.

For example:

```text
Sales
  │
  ▼
Legal
  │
  ▼
Rights
  │
  ▼
Operations
  │
  ▼
Finance
  │
  ▼
Customer
```

Each function may believe that its individual activity performs well.

However:

```text
Sales Activity       = 1 Hour
Legal Activity       = 2 Hours
Rights Activity      = 1 Hour
Operations Activity  = 2 Hours
Finance Activity     = 1 Hour

Total Work Time      = 7 Hours
```

while:

```text
Total End-to-End Lead Time = 18 Days
```

This immediately changes the improvement conversation.

The major opportunity may not be making each activity faster.

It may be reducing:

```text
Waiting

Queues

Handovers

Batching

Missing Information

Rework
```

---

# Information Flow

Value Stream Mapping should include the flow of information, not only the flow of work.

Lean Enterprise Institute explicitly includes information flow within Value Stream Mapping (Lean Enterprise Institute, n.d.a).

For each stage ask:

```text
What information tells this team what to do?

Where does that information come from?

How does it arrive?

Is it complete?

How long does the team wait for it?

Is the information manually transferred?

Does the same information need to be entered again?
```

For example:

```text
CRM
 │
 │ Contract Information
 ▼
Spreadsheet
 │
 │ Manual Re-key
 ▼
Finance System
 │
 │ Extract
 ▼
Reporting Platform
```

This may reveal that the true source of delay is information flow rather than the business activity itself.

---

# Information Flow and DISCOVER

This is particularly important for Data & Analytics discovery.

A value stream may appear to be:

```text
Business Process
```

but deeper discovery may reveal:

```text
Business Process
       │
       ▼
Information Dependency
       │
       ▼
Data Quality Problem
       │
       ▼
Manual Workaround
       │
       ▼
Process Delay
```

The improvement opportunity may therefore be a **Data Product**, not simply a process change.

---

# Lead Time

Lead Time measures the time required for work to move from the beginning to the end of a process or value stream.

Lean Enterprise Institute defines lead time as the time required for an item to move through a process or value stream from start to finish (Lean Enterprise Institute, n.d.a).

Example:

```text
Request Received

Monday 09:00

        ↓

Outcome Delivered

Friday 17:00
```

The elapsed lead time is significantly greater than the time someone actively works on the request.

---

# Processing Time

Processing Time represents the period during which work is actually being performed.

For example:

```text
Activity                  Processing Time

Validate Request          20 mins

Prepare Analysis          90 mins

Review Analysis           30 mins

Approve Analysis          15 mins

-----------------------------------------

Total Processing Time     155 mins
```

However:

```text
Total Lead Time = 5 Days
```

The difference between the two provides an important indicator of flow.

---

# Waiting Time

Waiting Time represents periods where work is not actively progressing.

Examples include:

```text
Waiting for Approval

Waiting for Data

Waiting for Customer Response

Waiting for Legal Review

Waiting for Batch Processing

Waiting for Month End

Waiting for System Update
```

Waiting may account for a significant proportion of end-to-end lead time.

---

# Queue

A queue occurs where work accumulates before the next activity.

For example:

```text
New Requests

Request 1
Request 2
Request 3
Request 4
Request 5

       │
       ▼

   Legal Review
```

Queues can indicate:

- Capacity constraints
- Batching
- Prioritisation problems
- Missing information
- Approval bottlenecks
- Skill constraints

---

# Rework

Rework occurs when an activity must be repeated or corrected.

For example:

```text
Contract Submitted
        │
        ▼
Contract Reviewed
        │
        ▼
Information Missing
        │
        ▼
Return to Sales
        │
        ▼
Contract Updated
        │
        ▼
Contract Reviewed Again
```

Rework increases lead time and consumes capacity.

Ask:

- Why was the information missing?
- Could the problem have been prevented upstream?
- How frequently does this occur?
- What information would prevent the failure?

---

# Handoffs

Each transfer of work creates a potential delay.

For example:

```text
Sales
  │
  ▼
Legal
  │
  ▼
Rights
  │
  ▼
Finance
```

For each handoff ask:

- What is transferred?
- How is it transferred?
- Is the recipient notified?
- Is information complete?
- Is information re-entered?
- Does the receiving team repeat validation?
- Does work enter a queue?

Reducing unnecessary handoffs can materially improve flow.

---

# Bottlenecks

A bottleneck constrains the ability of the overall value stream to deliver value.

Examples might include:

```text
Specialist Approval

Manual Reconciliation

Legal Review

Single Data Analyst

External Supplier

Legacy System

Monthly Batch Process
```

Optimising another part of the value stream may produce little benefit while the bottleneck remains.

This reinforces the importance of analysing the complete system.

---

# Value Stream Metrics

Useful measures may include:

| Measure | Description |
|---------|-------------|
| Lead Time | End-to-end elapsed time |
| Processing Time | Time actively spent performing work |
| Waiting Time | Time work is waiting |
| Queue Size | Work waiting to be processed |
| Volume | Number of items passing through |
| Error Rate | Percentage containing errors |
| Rework Rate | Percentage requiring repeated work |
| First-Time Quality | Percentage completed correctly first time |
| Automation Rate | Percentage handled automatically |
| Handoff Count | Number of ownership transfers |
| Cost | Cost of delivering the value stream |

Do not collect metrics simply because they are available.

Capture measures that help explain the performance of the value stream.

---

# Flow Efficiency

A useful analytical measure is the relationship between active processing time and total lead time.

Conceptually:

```text
Flow Efficiency

Processing Time
─────────────── × 100
  Lead Time
```

For example:

```text
Processing Time = 6 Hours

Lead Time       = 60 Hours


6
── × 100 = 10%
60
```

This suggests that the work is actively being progressed for only a small proportion of the overall elapsed time.

The figure should be used diagnostically rather than treated as a universal performance target.

---

# Mapping a Value Stream

A simple DISCOVER Value Stream Map may contain:

```text
Customer Need
      │
      ▼
Activity
      │
      ▼
Wait
      │
      ▼
Activity
      │
      ▼
Decision
      │
      ▼
Activity
      │
      ▼
Customer Outcome
```

Below the flow capture:

```text
Processing Time

Waiting Time

Lead Time

Quality

Volume

Pain Points
```

Above the flow capture:

```text
Information Sources

Systems

Decisions

Information Handovers
```

This provides a business-friendly representation without requiring complex Lean notation during early discovery.

---

# Example Value Stream

```text
CUSTOMER
   │
   │ Request
   ▼
┌──────────────┐
│ Receive      │
│ Request      │
└──────────────┘
   │
   │ Wait: 1 Day
   ▼
┌──────────────┐
│ Validate     │
│ Request      │
└──────────────┘
   │
   │ Wait: 2 Days
   ▼
┌──────────────┐
│ Prepare      │
│ Response     │
└──────────────┘
   │
   │ Wait: 3 Days
   ▼
┌──────────────┐
│ Approve      │
│ Response     │
└──────────────┘
   │
   ▼
CUSTOMER
RECEIVES VALUE
```

Timeline:

```text
Processing Time = 4 Hours

Waiting Time    = 6 Days

Lead Time       = 6 Days + 4 Hours
```

This makes the improvement opportunity visible immediately.

---

# Value Stream Mapping Workshop

A DISCOVER Value Stream Mapping workshop might follow this structure.

| Stage | Activity |
|-------|----------|
| 1 | Define customer / beneficiary |
| 2 | Define required value |
| 3 | Agree start and end points |
| 4 | Identify major activities |
| 5 | Map the current-state flow |
| 6 | Map information flow |
| 7 | Capture processing time |
| 8 | Capture waiting and queues |
| 9 | Identify handoffs |
| 10 | Identify rework |
| 11 | Identify bottlenecks |
| 12 | Classify activity |
| 13 | Capture pain points |
| 14 | Design future-state principles |
| 15 | Identify opportunities |
| 16 | Agree next steps |

The objective should be to understand the **whole value stream**, not to create a perfectly formatted diagram during the workshop.

---

# Workshop Participants

Value Stream Mapping should involve people from across the end-to-end flow.

Possible participants include:

- Value Stream Owner
- Business Owners
- Process Owners
- Operational Users
- Subject Matter Experts
- Product
- Data
- Technology
- Finance
- Relevant External Partners

Avoid allowing one department to map the complete value stream on behalf of everyone else.

Cross-functional participation is one of the strengths of the technique.

---

# Walk the Value Stream

Where possible, understand how work actually happens.

Do not rely solely on policy documents or senior stakeholder descriptions.

Ask operational users to demonstrate real examples.

For example:

> Show me the last request that came through this process.

Follow that request:

```text
Where did it arrive?

What happened next?

How long did it wait?

Who touched it?

Which system was used?

What information was missing?

Where was it transferred?

Was anything repeated?

What happened before the customer received the outcome?
```

Lean practice traditionally emphasises observing the actual work when creating a current-state map.

DISCOVER adopts the same principle.

---

# Generic Discovery Questions

## Customer and Value

- Who receives the final outcome?
- What do they value?
- What problem are they trying to solve?
- How do they measure a good outcome?
- What would cause dissatisfaction?

---

## Scope

- What starts the value stream?
- What ends it?
- Where should the map begin?
- Where should it stop?
- What outcome is produced?

---

## Flow

- What happens first?
- What happens next?
- Where does work stop?
- Where does it wait?
- Where does it move between teams?

---

## Information

- What information triggers each activity?
- Where does that information come from?
- How is it transferred?
- Is it complete?
- Is it trusted?
- Is information re-entered?

---

## Time

- How long does each activity take?
- How long does work wait?
- What is the total lead time?
- Which activity causes the most delay?
- Are activities performed continuously or in batches?

---

## Quality

- Where do errors occur?
- Where does rework occur?
- Which information is frequently incomplete?
- How often does work need to go backwards?
- What percentage succeeds first time?

---

## Ownership

- Who owns the complete value stream?
- Who owns each stage?
- Where does accountability transfer?
- Is end-to-end accountability clear?

---

## Technology

- Which systems support the flow?
- Where is information manually moved?
- Where are spreadsheets used?
- Are systems integrated?
- Does technology create waiting or batching?

---

## Improvement

- Which activities genuinely create value?
- Which activities are required controls?
- Which activities appear unnecessary?
- Where could waiting be removed?
- Where could handoffs be simplified?
- What information would improve flow?
- What could be automated?
- Where could AI augment human work?

---

# Identifying Waste

During discovery look for recurring patterns of waste.

Examples include:

## Waiting

```text
Waiting for approval

Waiting for information

Waiting for system processing
```

---

## Rework

```text
Correcting data

Repeating reconciliation

Resubmitting requests
```

---

## Duplication

```text
Entering the same information twice

Maintaining duplicate spreadsheets

Producing duplicate reports
```

---

## Unnecessary Handoffs

```text
Work transferred between multiple teams without adding value
```

---

## Over-Processing

```text
Multiple checks of the same information

Excessive reporting

Repeated formatting
```

---

## Unused Output

```text
Reports nobody consumes

Data collected but never used
```

---

## Searching

```text
Searching for documents

Finding the right data

Locating the correct definition
```

These categories provide prompts for discovery.

They should not be used to prejudge the value of an activity before its purpose is understood.

---

# Future-State Design Questions

Once the current state has been understood ask:

```text
What could disappear?

What could happen earlier?

What could happen automatically?

What could happen in parallel?

What information could be available sooner?

What approval could become risk based?

What handoff could disappear?

What could be standardised?

What could become self-service?
```

The resulting future state should address root causes rather than merely make the existing workflow faster.

---

# Prioritising Improvements

Do not attempt to fix every issue simultaneously.

Potential improvements can be assessed against:

```text
Business Value

Customer Impact

Lead-Time Reduction

Quality Improvement

Effort

Cost

Risk

Dependencies
```

This can feed directly into the DISCOVER Opportunity Register and Prioritisation process.

---

# Connecting Value Streams to POPIT-V

Value Stream Mapping cuts across every POPIT-V dimension.

## People

- Who performs the work?
- Where is specialist knowledge required?
- Who makes decisions?
- Where does workload accumulate?

## Organisation

- Which teams participate?
- Who owns the complete value stream?
- Where do organisational boundaries interrupt flow?

## Process

- What activities occur?
- Where does work wait?
- Where are bottlenecks and rework?

## Information

- What information enables flow?
- Where is information missing?
- Where are definitions inconsistent?

## Technology

- Which systems enable the flow?
- Where do systems create constraints?
- Where is manual integration required?

## Value

- Who receives value?
- What outcome matters?
- Which activities contribute towards that outcome?
- What improvement would create measurable benefit?

---

# Connecting Value Streams to Business Capabilities

A value stream normally crosses multiple capabilities.

For example:

```text
VALUE STREAM

Licence Programme to Customer

            │
            ▼

Sales Management
            │
            ▼
Contract Management
            │
            ▼
Rights Management
            │
            ▼
Content Delivery
            │
            ▼
Revenue Management
            │
            ▼
Customer Receives Value
```

This helps identify which capabilities contribute towards an end-to-end business outcome.

A useful relationship is:

```text
Strategy
   │
   ▼
Value Stream
   │
   ▼
Capabilities
   │
   ▼
Processes
```

Capability Mapping and Value Stream Mapping therefore provide complementary views of the organisation.

---

# Connecting Value Streams to Process Modelling

Once a problematic section of the value stream has been identified, Process Modelling can be used to investigate it in more detail.

For example:

```text
VALUE STREAM

Contract Review
     │
     │
     │  ← Major Delay Identified
     ▼

PROCESS MODELLING

Receive Contract
      │
      ▼
Check Completeness
      │
      ▼
Legal Review
      │
      ▼
Commercial Review
      │
      ▼
Approval
```

The value stream identifies **where to investigate**.

Process Modelling explains **how that part works**.

---

# Connecting Value Streams to Event Storming

Event Storming can be used to discover how value progresses through a complex business domain.

For example:

```text
Opportunity Created

Contract Signed

Rights Granted

Programme Delivered

Invoice Issued

Revenue Recognised
```

These events can provide the initial backbone of a Value Stream Map.

The techniques therefore complement each other:

```text
Event Storming
      │
      ▼
Discover Significant Events
      │
      ▼
Value Stream Mapping
      │
      ▼
Understand End-to-End Flow
```

---

# Connecting Value Streams to Data Products

A particularly important DISCOVER application is understanding how information affects value flow.

Consider:

```text
Business Decision
      │
      ▼
Information Required
      │
      ▼
Information Unavailable
      │
      ▼
Work Waits
```

This may indicate an opportunity for a Data Product.

For example:

```text
Rights Availability Decision
        │
        ▼
Need Contract + Territory + Rights Data
        │
        ▼
Data Located Across Multiple Systems
        │
        ▼
Manual Investigation
        │
        ▼
2-Day Delay
```

Potential response:

```text
Rights Availability Data Product
```

The Data Product creates value because it improves the performance of the value stream.

---

# Connecting Value Streams to Decisions

A value stream should also expose important decisions.

For example:

```text
Opportunity Received
      │
      ▼
Can We Sell This Programme?
      │
      ▼
Rights Decision
      │
      ▼
What Price Should We Offer?
      │
      ▼
Commercial Decision
```

For each decision ask:

```text
Who makes it?

What information is required?

How long does it take?

What happens when information is unavailable?

Could better data improve the decision?
```

This reinforces the DISCOVER principle:

> **Decisions drive data requirements.**

---

# Connecting Value Streams to AI

Value Stream Mapping can expose activities where AI may improve flow.

Possible areas include:

```text
Searching

Reading

Classification

Summarisation

Prediction

Recommendation

Reconciliation

Monitoring

Content Generation
```

For example:

```text
Contract Received
      │
      ▼
Manual Review
      │
      │  2-Day Queue
      ▼
Rights Extracted
```

Potential opportunity:

```text
AI-Assisted Contract Review
+
Rights Metadata Extraction
```

Another example:

```text
Month-End Actuals
      │
      ▼
Manual Variance Analysis
      │
      ▼
Manual Commentary
```

Potential opportunities:

```text
Anomaly Detection

Variance Explanation

Financial Commentary Assistant
```

AI should only be recommended where it improves the value stream and produces sufficient business value.

The DISCOVER AI Opportunity Canvas should be used to assess the opportunity separately.

---

# Finance Example

## Discovery Objective

Understand the end-to-end flow from commercial agreement through to recognised and reported revenue.

An initial value stream might look like:

```text
Commercial
Agreement
    │
    ▼
Contract
Signed
    │
    │  Wait
    ▼
Contract
Received by Finance
    │
    ▼
Revenue Rules
Reviewed
    │
    │  Manual Work
    ▼
Revenue Schedule
Created
    │
    ▼
Invoice
Created
    │
    ▼
Revenue
Recognised
    │
    │  Reconciliation
    ▼
Actuals
Reported
    │
    ▼
Management
Reporting
```

### Example Questions

- What triggers the revenue value stream?
- Where does Finance first receive contract information?
- How long after signature does Finance receive it?
- What information is usually missing?
- Which revenue rules require manual interpretation?
- Where are spreadsheets used?
- Where does information need to be re-entered?
- Which activities wait for month-end?
- Where are reconciliations required?
- Where does rework occur?
- Which stages create the most lead time?
- Who owns the complete value stream?

### Potential Findings

Discovery may reveal:

```text
Contract information reaches Finance late.

Contract data must be manually interpreted.

Revenue rules vary by deal type.

Information is copied into spreadsheets.

Finance performs repeated reconciliation.

Actuals and forecast data use different structures.

Management reporting requires further manual consolidation.
```

### Potential Opportunities

- Contract Data Product
- Revenue Data Product
- Revenue Recognition Rules Catalogue
- Automated Contract Metadata Extraction
- Automated Reconciliation
- Finance Semantic Layer
- Forecast vs Actual Monitoring
- Automated Management Commentary

---

# Marketing Example

## Discovery Objective

Understand the end-to-end flow from campaign need through to learning and optimisation.

A possible value stream:

```text
Marketing
Objective
   │
   ▼
Campaign
Brief
   │
   │ Wait for Approval
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
   │ Wait
   ▼
Campaign
Launched
   │
   ▼
Performance
Data Received
   │
   │ Manual Consolidation
   ▼
Campaign
Analysed
   │
   ▼
Learning
Captured
   │
   ▼
Next Campaign
Improved
```

### Example Questions

- What triggers campaign activity?
- How long does planning take?
- Where are approvals required?
- Where does work queue?
- How quickly can campaigns launch?
- How quickly is performance information available?
- Is campaign information consolidated manually?
- How long before optimisation decisions can be made?
- Is historical learning available when new campaigns are planned?
- Where are the major handovers between Marketing, agencies and Data?
- What does the end customer value?

### Potential Findings

Discovery may reveal:

```text
Campaign approval introduces delay.

Audience information exists in several systems.

Creative approval requires repeated handoffs.

Performance information arrives at different times.

Analysts manually consolidate platform data.

Historical campaign learning is difficult to find.

Optimisation occurs too late to affect campaign performance.
```

### Potential Opportunities

- Campaign Performance Data Product
- Audience Data Product
- Marketing Semantic Layer
- Automated Campaign Data Integration
- Campaign Performance Alerts
- Predictive Campaign Optimisation
- Campaign Knowledge Assistant

---

# Value Stream Ownership

A recurring discovery finding may be that individual processes have owners but the end-to-end value stream does not.

For example:

```text
Sales Process
Owner = Sales

Contract Process
Owner = Legal

Billing Process
Owner = Finance

Delivery Process
Owner = Operations
```

But:

```text
End-to-End Customer Outcome

Owner = ?
```

This can create local optimisation and fragmented accountability.

Where appropriate, DISCOVER should identify whether end-to-end value stream ownership is required.

---

# Value Stream Mapping for Data & Analytics

Data and analytics can themselves have value streams.

For example:

```text
Business Question
      │
      ▼
Data Requested
      │
      ▼
Data Located
      │
      ▼
Data Extracted
      │
      ▼
Data Prepared
      │
      ▼
Analysis Created
      │
      ▼
Insight Delivered
      │
      ▼
Decision Made
```

Discovery may reveal:

```text
3 Hours Analysis

+

10 Days Waiting for Data
```

This suggests that improving analytical productivity alone may not materially improve the business outcome.

The larger opportunity may be:

```text
Governed Data Product

Self-Service Data

Semantic Layer

Improved Access

Automated Data Pipeline
```

This makes Value Stream Mapping particularly relevant to Data Product Discovery.

---

# Value Stream Mapping for AI

AI value streams can similarly be considered end to end.

For example:

```text
Business Need
      │
      ▼
Information Gathered
      │
      ▼
Human Analysis
      │
      ▼
Decision
      │
      ▼
Action
      │
      ▼
Outcome
```

Do not examine only:

```text
Human Analysis
```

and assume AI is the solution.

The real constraint may be upstream:

```text
Information unavailable

Poor data quality

Unclear business rules

Approval delays
```

Value Stream Mapping helps identify where AI would genuinely change the overall outcome rather than simply accelerating one isolated task.

---

# Common Pitfalls

## Mapping Processes Instead of the Value Stream

Do not become trapped in detailed process activity too early.

The purpose is to understand the **end-to-end flow**.

---

## Mapping Departments

A value stream should not simply become:

```text
Sales → Finance → Technology → Operations
```

Capture what happens and how value flows across those boundaries.

---

## Ignoring Information Flow

Information can be the primary reason work stops.

Map it explicitly.

---

## Ignoring Waiting

A map containing only activities hides much of the value stream.

Waiting and queues are critical.

---

## Using Estimated Times as Facts

Stakeholders may estimate processing and waiting times.

Clearly distinguish:

```text
Measured

Estimated

Unknown
```

Validate important figures where possible.

---

## Assuming Every Non-Value-Adding Activity Should Disappear

Some activities exist for legitimate:

```text
Regulatory

Legal

Financial

Security

Risk
```

reasons.

The objective may be simplification rather than elimination.

---

## Optimising One Step

Improving one process does not necessarily improve the whole value stream.

Always assess the end-to-end effect.

---

## Designing the Future State Too Early

Understand the current state first.

Otherwise proposed solutions may address symptoms rather than causes.

---

## Automating Waste

Before automating an activity ask:

```text
Should this activity exist at all?
```

---

## Creating a Beautiful Map With No Action

The purpose of Value Stream Mapping is improvement.

The map should lead towards:

```text
Findings

Opportunities

Future State

Actions

Priorities

Roadmap
```

---

# What Good Looks Like

An effective Value Stream Map should:

- Have a clearly defined customer or beneficiary
- Define the value being delivered
- Have clear start and end points
- Show the major end-to-end activities
- Cross organisational boundaries
- Show important information flows
- Show relevant handoffs
- Capture waiting and queues
- Capture processing time where useful
- Identify rework
- Identify bottlenecks
- Identify significant controls
- Highlight pain points
- Identify improvement opportunities
- Be based on actual current-state understanding
- Support future-state design
- Connect improvements to measurable value

Most importantly, the map should help stakeholders see **the whole system rather than isolated parts**.

---

# Discovery Outputs

Value Stream Mapping should contribute to:

- Current-State Value Stream Map
- Future-State Value Stream Map
- Value Stream Catalogue
- Value Stream Ownership
- Lead-Time Analysis
- Bottleneck Analysis
- Information Flow Analysis
- Waste Analysis
- Pain Point Register
- Opportunity Register
- Process Improvement Opportunities
- Data Product Opportunities
- AI Opportunities
- Benefit Measures
- Roadmap

---

# Related DISCOVER Techniques

Value Stream Mapping works particularly well alongside:

- Business Capability Mapping
- Stakeholder Mapping
- Process Modelling
- Event Storming
- Business Glossary
- Ontology Discovery
- Root Cause Analysis
- Data Product Design
- Prioritisation

A common progression might be:

```text
Business Strategy
       │
       ▼
Business Outcome
       │
       ▼
Value Stream
       │
       ▼
Current State
       │
       ├────────────► Capabilities
       ├────────────► Processes
       ├────────────► Information
       ├────────────► Technology
       ├────────────► Decisions
       └────────────► Pain Points
                           │
                           ▼
                       Opportunities
                           │
                  ┌────────┴────────┐
                  ▼                 ▼
             Data Products         AI
                  │                 │
                  └────────┬────────┘
                           ▼
                     Future State
                           │
                           ▼
                        Roadmap
```

The exact sequence should depend upon the discovery engagement.

---

# Recommended Discovery Questions – Quick Reference

Before concluding Value Stream Mapping, ensure you can answer:

- Who is the customer or beneficiary?
- What value are they expecting?
- What starts the value stream?
- What ends it?
- What are the major activities?
- What is the total lead time?
- How much time is active processing?
- Where does work wait?
- Where do queues form?
- Where are handoffs?
- Where does rework occur?
- What information enables the flow?
- Where is information missing?
- Which systems support the flow?
- Where is information manually transferred?
- Which activities create value?
- Which activities are necessary controls?
- Which activities appear unnecessary?
- What is the major bottleneck?
- Who owns the end-to-end value stream?
- Which decisions slow the flow?
- What Data Products could improve the flow?
- Where could automation help?
- Where could AI create meaningful value?
- What should the future state look like?
- How will improvement be measured?

---

# References

International Institute of Business Analysis (IIBA) (n.d.a) *7.23 Value Stream Mapping*. Agile Extension to the BABOK® Guide. Available at: https://www.iiba.org/knowledgehub/agile-extension/7-techniques/7-23-value-stream-mapping/ (Accessed: 10 August 2026).

International Institute of Business Analysis (IIBA) (n.d.b) *11.4 The Business Architecture Perspective*. A Guide to the Business Analysis Body of Knowledge (BABOK® Guide). Available at: https://www.iiba.org/knowledgehub/business-analysis-body-of-knowledge-babok-guide/11-perspectives/11-4-the-business-architecture-perspective/ (Accessed: 10 August 2026).

International Institute of Business Analysis (IIBA) (n.d.c) *10.34 Process Analysis*. A Guide to the Business Analysis Body of Knowledge (BABOK® Guide). Available at: https://www.iiba.org/knowledgehub/business-analysis-body-of-knowledge-babok-guide/10-techniques/10-34-process-analysis/ (Accessed: 10 August 2026).

International Organization for Standardization (ISO) (2020) *ISO 22468:2020 Value stream management (VSM)*. Geneva: International Organization for Standardization.

Lean Enterprise Institute (n.d.a) *Value Stream Mapping Overview*. Available at: https://www.lean.org/lexicon-terms/value-stream-mapping/ (Accessed: 10 August 2026).

Lean Enterprise Institute (n.d.b) *Lean Thinking and Practice*. Available at: https://www.lean.org/lexicon-terms/lean-thinking-and-practice/ (Accessed: 10 August 2026).

Lean Enterprise Institute (2022) *Understanding the Fundamentals of Value-Stream Mapping*. Available at: https://www.lean.org/the-lean-post/articles/understanding-the-fundamentals-of-value-stream-mapping/ (Accessed: 10 August 2026).

Rother, M. and Shook, J. (1999) *Learning to See: Value-Stream Mapping to Create Value and Eliminate Muda*. Cambridge, MA: Lean Enterprise Institute.