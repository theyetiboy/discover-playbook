---
title: "Event Storming"
version: "1.0"
author: "Steve Tarry"
technique: "Discovery Technique"
---

# Event Storming

## Purpose

Event Storming is a collaborative modelling technique used to explore complex business domains by identifying significant things that happen within the business and arranging them into a meaningful sequence.

The technique was created by Alberto Brandolini in 2013 and was initially developed as a way of modelling complex business processes using ideas associated with Domain-Driven Design. It has subsequently evolved into a broader collaborative modelling technique that can be applied to organisations, processes, services and software (Brandolini, n.d.a).

Within DISCOVER, Event Storming is primarily used as a **business discovery technique**.

It helps practitioners:

- Understand complex business workflows
- Discover important business events
- Identify business rules
- Surface hidden assumptions
- Understand decision points
- Reveal dependencies and handovers
- Identify pain points and bottlenecks
- Discover important business concepts
- Build shared understanding across teams
- Identify candidate domain boundaries
- Support ontology development
- Identify Data Product and AI opportunities

Event Storming is particularly valuable when no single stakeholder understands the entire end-to-end process.

---

# Why This Technique Matters

Traditional process discovery often involves interviewing individuals separately and then attempting to reconstruct the process afterwards.

This approach can miss:

- Different perspectives
- Hidden dependencies
- Conflicting assumptions
- Informal workarounds
- Exceptions
- Undocumented knowledge

Event Storming deliberately brings different perspectives together.

Brandolini describes EventStorming as an act of **deliberate collective learning**, where participants collaboratively explore a complex domain rather than relying on one person to describe it (Brandolini, 2016).

The visual nature of the technique allows participants to see the business flow together and challenge the emerging model.

This makes Event Storming particularly useful for DISCOVER because discovery is intended to create **shared understanding**, not simply documentation.

---

# When to Use Event Storming

Event Storming is particularly useful when:

- A business process is complex
- Multiple teams participate in the same workflow
- Business rules are poorly documented
- Different stakeholders describe the process differently
- There are many exceptions
- Ownership changes throughout the process
- Multiple systems support the workflow
- Significant manual intervention exists
- An unfamiliar business domain needs to be understood quickly
- Domain boundaries are unclear
- An Enterprise Ontology is being developed
- New Data Products are being considered
- AI or automation opportunities are being explored

It can also be useful when stakeholders repeatedly say:

> "It's complicated."

or:

> "You'll need to speak to several people to understand that."

Those statements often indicate that collaborative exploration will provide more value than a sequence of isolated interviews.

---

# Start With Events

The fundamental building block of Event Storming is the **Domain Event**.

A Domain Event represents something meaningful that has happened within the business.

Events should normally be expressed in the past tense.

Examples:

```text
Contract Signed

Campaign Approved

Programme Commissioned

Rights Granted

Invoice Issued

Revenue Recognised

Payment Received

Forecast Updated
```

The event should describe something that has occurred rather than an activity someone intends to perform.

For example:

```text
Poor

Approve Contract
```

This describes an action.

A corresponding event might be:

```text
Contract Approved
```

The distinction becomes increasingly useful as the model develops.

---

# Event Storming Mindset

Participants should initially focus on:

> **What happens in the business?**

rather than:

> **Which system performs this?**

or:

> **How should we redesign it?**

Technology and improvement opportunities can be layered onto the model after the business flow is understood.

This aligns strongly with the DISCOVER principle:

> **Understand before recommending.**

---

# Big Picture Discovery

One of the most useful applications of Event Storming during early discovery is exploring the **Big Picture**.

The objective is to understand the major events occurring across a business domain without immediately modelling every detailed process step.

For example:

```text
Programme
Commissioned

      ↓

Production
Started

      ↓

Programme
Delivered

      ↓

Rights
Confirmed

      ↓

Licence
Agreed

      ↓

Content
Delivered

      ↓

Invoice
Issued

      ↓

Revenue
Recognised
```

This immediately starts a conversation.

Participants may challenge:

- The sequence
- Missing events
- Ownership
- Terminology
- Dependencies
- Exceptions

That conversation is the value of Event Storming.

---

# Building the Timeline

Business events are placed approximately in chronological order.

For example:

```text
Opportunity
Created
    │
    ▼
Customer
Qualified
    │
    ▼
Proposal
Submitted
    │
    ▼
Contract
Negotiated
    │
    ▼
Contract
Signed
    │
    ▼
Service
Delivered
    │
    ▼
Invoice
Issued
    │
    ▼
Payment
Received
```

The process does not need to be perfect initially.

Participants should add events rapidly and refine the sequence collaboratively.

---

# Commands

Once important events are visible, explore what caused them.

A **Command** represents an action or intention that may result in an event.

For example:

```text
COMMAND

Approve Contract

      │
      ▼

EVENT

Contract Approved
```

Another example:

```text
COMMAND

Issue Invoice

      │
      ▼

EVENT

Invoice Issued
```

Commands help identify:

- User actions
- System actions
- Responsibilities
- Process steps
- Automation opportunities

---

# Actors

An Actor represents the person or role responsible for initiating an action.

For example:

```text
Finance Analyst
       │
       ▼
Post Journal
       │
       ▼
Journal Posted
```

Actors may include:

- Customer
- Sales Executive
- Finance Analyst
- Marketing Manager
- Rights Executive
- Producer
- System
- External Partner

Identifying actors helps connect Event Storming to the **People** perspective of POPIT-V.

---

# Business Rules and Policies

Some events trigger decisions or rules that determine what happens next.

For example:

```text
Contract Signed
       │
       ▼
Check Revenue
Recognition Rules
       │
       ▼
Revenue Recognition
Scheduled
```

Useful questions include:

- Why does this happen?
- Under what conditions?
- Are there exceptions?
- Who decides?
- Is the rule documented?
- Does the rule vary by territory, product or customer?

Business rules discovered here should also be captured within the appropriate DISCOVER artefacts.

---

# External Systems

External systems can be added when they materially affect the business flow.

Examples might include:

```text
CRM

ERP

Rights Platform

Marketing Platform

Payment Provider

External Research Provider
```

The purpose is not initially to create an architecture diagram.

The objective is to expose:

- Dependencies
- Handovers
- Integration points
- Manual transfers
- Ownership boundaries

---

# Hot Spots

A particularly valuable part of Event Storming is capturing areas of uncertainty, disagreement or concern.

DISCOVER refers to these as **Hot Spots**.

Examples:

```text
Nobody knows who approves this.

This calculation changes by territory.

This step is performed manually.

Marketing and Finance disagree on the definition.

This sometimes takes three weeks.

We don't know which system owns this value.
```

Do not immediately resolve every Hot Spot.

Capture it visibly.

A Hot Spot is a discovery finding.

It may later become:

- A question
- A pain point
- A risk
- An assumption
- A business rule
- An opportunity
- A separate discovery session

---

# Important Business Concepts

As events are explored, important business concepts naturally emerge.

For example:

```text
Customer

Contract

Programme

Rights

Territory

Invoice

Revenue
```

These concepts should be captured for further analysis.

Event Storming therefore provides valuable input into:

- Business Glossary
- Domain-Driven Design
- Ontology Discovery
- Data Modelling
- Data Product Design

---

# A Simple Event Storming Model

A simplified model might look like:

```text
ACTOR
Sales Executive

      │

      ▼

COMMAND
Create Opportunity

      │

      ▼

EVENT
Opportunity Created

      │

      ▼

COMMAND
Submit Proposal

      │

      ▼

EVENT
Proposal Submitted

      │

      ▼

COMMAND
Approve Contract

      │

      ▼

EVENT
Contract Approved

      │

      ▼

COMMAND
Sign Contract

      │

      ▼

EVENT
Contract Signed
```

Additional information can then be layered around this flow.

---

# Event Storming Workshop

A DISCOVER Event Storming workshop might follow the structure below.

| Stage | Activity |
|-------|----------|
| 1 | Confirm scope |
| 2 | Explain Domain Events |
| 3 | Allow participants to identify events |
| 4 | Arrange events chronologically |
| 5 | Identify missing events |
| 6 | Identify commands and actors |
| 7 | Capture business rules |
| 8 | Identify external systems |
| 9 | Capture Hot Spots |
| 10 | Identify important business concepts |
| 11 | Identify pain points and opportunities |
| 12 | Playback the complete flow |

The facilitator should avoid trying to control the model too early.

The initial objective is discovery.

Structure comes later.

---

# Preparing the Workshop

Before the workshop:

- Define the business domain
- Agree the scope
- Invite representatives from across the process
- Include operational Subject Matter Experts
- Include relevant decision makers
- Prepare a large physical or virtual workspace
- Provide clear modelling instructions
- Explain that disagreement is useful

Avoid providing a completed process map beforehand.

Doing so may anchor participants to an existing interpretation of the business.

---

# Who Should Attend?

Event Storming works best when participants represent different perspectives.

Possible attendees include:

- Business Owners
- Product Managers
- Operational Users
- Subject Matter Experts
- Analysts
- Data Specialists
- Architects
- Engineers
- Process Owners
- System Owners

Brandolini's EventStorming approach deliberately encourages cross-discipline collaboration between stakeholders with different backgrounds (Brandolini, n.d.a).

The exact participants should depend upon the discovery objective.

---

# Facilitation

The facilitator should focus on creating conversation.

Useful prompts include:

- What happens next?
- What happened before this?
- Who causes this to happen?
- Why does this happen?
- What information is needed?
- What could prevent this?
- What happens if it fails?
- Does this always happen?
- Who disagrees with this?
- What are we missing?

Avoid becoming the person who creates the entire model.

The model belongs to the participants.

---

# Generic Discovery Questions

## Events

- What significant things happen within this process?
- What happens first?
- What happens next?
- What marks the end of the process?
- Which events are particularly important?

---

## Triggers

- What causes this event?
- Who initiates it?
- Is it triggered manually or automatically?
- Can several different triggers cause the same event?

---

## Actors

- Who performs this action?
- Who owns the outcome?
- Who approves it?
- Who needs to know that it happened?

---

## Decisions

- Where are decisions made?
- What information is required?
- Who makes the decision?
- Which rules apply?
- Can the decision be reversed?

---

## Exceptions

- What happens when the normal flow fails?
- Which exceptions occur frequently?
- What requires manual intervention?
- What causes work to stop?

---

## Information

- What information is required at this point?
- What information is created?
- Where does it originate?
- Who owns it?
- Can it be trusted?

---

## Technology

- Which system supports this event?
- Does information move between systems?
- Is data manually re-entered?
- Are spreadsheets or email involved?

---

## Pain Points

- Where does the process slow down?
- Where does rework occur?
- Which events generate the most problems?
- Where is ownership unclear?

---

## Opportunities

- What could be automated?
- What information would improve this step?
- Could a Data Product support this decision?
- Could AI assist this activity?
- Which unnecessary steps could potentially be removed?

---

# Connecting Event Storming to POPIT-V

Event Storming naturally exposes all six POPIT-V perspectives.

## People

- Who performs commands?
- Who makes decisions?
- Who owns outcomes?

## Organisation

- Which teams participate?
- Where do ownership boundaries exist?
- Which governance rules apply?

## Process

- What happens?
- In what sequence?
- Where are exceptions and handovers?

## Information

- What information is created?
- What information is consumed?
- What concepts and business rules exist?

## Technology

- Which systems enable each activity?
- Where do integrations occur?
- Where is manual intervention required?

## Value

- Which events create value?
- Which activities introduce delay?
- Which improvements would have the greatest impact?

---

# Connecting Event Storming to DDD

Event Storming and Domain-Driven Design complement each other closely.

Event Storming may reveal:

```text
Events

Commands

Actors

Business Rules

Concepts

Boundaries
```

These can then support discovery of:

```text
Domains

Subdomains

Ubiquitous Language

Entities

Bounded Contexts

Context Relationships
```

For example:

```text
Contract Signed
      │
      ▼
Rights Granted
      │
      ▼
Content Licensed
      │
      ▼
Revenue Recognised
```

may reveal several different business contexts:

```text
Contract Management

Rights Management

Content Sales

Finance
```

The transitions between those areas may indicate potential domain boundaries requiring further investigation.

---

# Connecting Event Storming to Ontology Discovery

Events expose relationships between business concepts.

For example:

```text
Customer
    │
    ▼
Signs
    │
    ▼
Contract

Contract
    │
    ▼
Grants
    │
    ▼
Rights

Rights
    │
    ▼
Apply To
    │
    ▼
Programme
```

These relationships can become candidates for the Enterprise Ontology.

Event Storming therefore helps discover not only **what concepts exist**, but also **how they interact over time**.

---

# Connecting Event Storming to Process Modelling

Event Storming and formal Process Modelling serve different purposes.

Event Storming is primarily exploratory.

Process Modelling is generally more structured and descriptive.

A useful DISCOVER pattern is:

```text
Event Storming
      │
      ▼
Discover Reality
      │
      ▼
Validate Flow
      │
      ▼
Process Modelling
      │
      ▼
Document Agreed Process
```

Trying to create a perfect BPMN diagram while stakeholders are still discovering how the business works can slow down exploration.

Event Storming provides a more flexible starting point.

---

# Connecting Event Storming to Data Products

Important events frequently reveal valuable Data Product opportunities.

For example:

```text
Forecast Updated

Revenue Recognised

Rights Granted

Campaign Completed
```

may lead to products such as:

```text
Forecast Performance Data Product

Revenue Performance Data Product

Rights Availability Data Product

Campaign Performance Data Product
```

Useful questions include:

- Which events do decision makers need visibility of?
- Which events need near-real-time reporting?
- Which events are difficult to reconcile?
- Which events require information from several domains?

---

# Connecting Event Storming to AI

Event Storming can also expose activities suitable for AI support.

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

might reveal opportunities for:

```text
Contract Summarisation

Metadata Extraction

Rights Classification
```

Or:

```text
Forecast Updated
      │
      ▼
Performance Reviewed
      │
      ▼
Commentary Produced
```

might reveal opportunities for:

```text
Anomaly Detection

Forecasting

Automated Commentary
```

AI opportunities should still be evaluated using the DISCOVER AI Opportunity Canvas before being recommended.

---

# Finance Example

## Discovery Objective

Understand the end-to-end revenue lifecycle and identify rules, ownership, information dependencies and improvement opportunities.

An initial timeline might include:

```text
Contract
Signed
   │
   ▼
Billing Schedule
Created
   │
   ▼
Invoice
Issued
   │
   ▼
Revenue
Recognised
   │
   ▼
Actuals
Posted
   │
   ▼
Forecast
Updated
   │
   ▼
Period
Closed
```

### Questions

- What happens when a contract is signed?
- When does Finance first become aware of it?
- What determines when an invoice can be issued?
- What determines when revenue can be recognised?
- Which rules vary by contract?
- Which rules vary by territory?
- Where are manual adjustments introduced?
- What happens when actual revenue differs from forecast?
- What triggers reconciliation?
- Who approves adjustments?

### Potential Hot Spots

```text
Sales contract information arrives late.

Revenue rules differ by contract type.

Manual spreadsheet used for adjustments.

Finance and Sales forecasts do not reconcile.

Exchange-rate treatment is unclear.

Revenue ownership changes during the lifecycle.
```

### Potential Concepts

```text
Contract
Customer
Revenue
Invoice
Forecast
Actual
Currency
Territory
Royalty
```

### Potential Opportunities

- Revenue Data Product
- Automated Reconciliation
- Revenue Recognition Rules Catalogue
- Forecast Variance Monitoring
- Finance Knowledge Assistant
- Automated Financial Commentary

---

# Marketing Example

## Discovery Objective

Understand the end-to-end campaign lifecycle and identify information, decision and measurement opportunities.

A simplified flow might include:

```text
Campaign
Brief Created
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
Campaign
Launched
   │
   ▼
Impressions
Delivered
   │
   ▼
Engagement
Recorded
   │
   ▼
Campaign
Completed
   │
   ▼
Performance
Reviewed
```

### Questions

- What triggers a campaign?
- Who approves the brief?
- How is budget approved?
- How are audiences selected?
- Which platforms execute the campaign?
- What performance events are captured?
- When is a campaign considered complete?
- How is success evaluated?
- How is attribution performed?
- What happens to learning from previous campaigns?

### Potential Hot Spots

```text
Campaign identifiers differ between platforms.

Audience definitions are inconsistent.

Performance data arrives at different times.

Attribution rules are disputed.

Reporting requires manual consolidation.

Historical campaign knowledge is difficult to retrieve.
```

### Potential Concepts

```text
Campaign
Audience
Segment
Channel
Creative
Impression
Engagement
Conversion
Spend
Revenue
```

### Potential Opportunities

- Campaign Performance Data Product
- Audience 360
- Automated Campaign Reporting
- Campaign Knowledge Assistant
- Performance Anomaly Detection
- AI Campaign Recommendations

---

# Remote Event Storming

Event Storming can also be facilitated remotely.

A collaborative digital workspace can be used to represent:

- Events
- Commands
- Actors
- Rules
- Systems
- Hot Spots

Remote facilitation requires particular attention to:

- Participant engagement
- Workspace navigation
- Clear instructions
- Breaks
- Group size
- Facilitation discipline

The modelling principles remain the same.

---

# Common Pitfalls

## Turning It Into Process Documentation Too Early

Event Storming is primarily exploratory.

Do not worry initially about perfect formatting.

Discover first.

Formalise later.

---

## Inviting Only Technology People

The value comes from cross-functional business knowledge.

Ensure Domain Experts and operational participants are present.

---

## Following the Happy Path Only

Ask:

> What happens when this doesn't work?

Exceptions often reveal the greatest complexity.

---

## Starting With Systems

Avoid:

```text
Salesforce sends data to Oracle.
```

Start with:

```text
Contract Signed
```

Then determine which systems enable that business event.

---

## Solving Every Problem Immediately

Capture Hot Spots.

Do not allow every discovery finding to become a 30-minute solution-design conversation.

---

## Facilitator Dominance

The facilitator should enable the conversation rather than provide the answers.

---

## Excessive Detail

Begin with the Big Picture.

Zoom into specific areas only when deeper understanding provides value.

---

## Ignoring Disagreement

Disagreement is useful.

It often reveals:

- Semantic differences
- Domain boundaries
- Hidden rules
- Ownership problems
- Process variations

Capture it rather than attempting to suppress it.

---

# What Good Looks Like

Effective Event Storming should result in:

- Shared understanding of the business flow
- Major Domain Events identified
- Important actors identified
- Commands understood
- Business rules exposed
- Exceptions captured
- Hot Spots documented
- Important concepts identified
- Domain boundaries suggested
- Pain points visible
- Opportunities captured
- Follow-up questions agreed

Participants should leave the workshop understanding more about the business than they did when they entered.

---

# Discovery Outputs

Event Storming should contribute to:

- Event Catalogue
- Process Maps
- Business Glossary
- Business Rules Catalogue
- Domain Model
- Context Map
- Ontology Capture
- Pain Point Register
- Opportunity Register
- Data Product Opportunities
- AI Opportunities
- Follow-Up Discovery Plan

---

# Related DISCOVER Techniques

Event Storming works particularly well alongside:

- Business Capability Mapping
- Business Glossary
- Domain-Driven Design
- Ontology Discovery
- Process Modelling
- Stakeholder Mapping
- Value Stream Mapping

A common progression might be:

```text
Capability Mapping
        │
        ▼
Business Domain Identified
        │
        ▼
Event Storming
        │
        ▼
Business Events & Rules
        │
        ├──────────────► Process Model
        │
        ├──────────────► Business Glossary
        │
        ├──────────────► Domain Model
        │
        └──────────────► Ontology
                              │
                              ▼
                         Opportunities
```

This sequence is illustrative rather than mandatory.

DISCOVER techniques should be selected according to the needs of the engagement.

---

# Recommended Discovery Questions – Quick Reference

Before concluding Event Storming, ensure you can answer:

- What starts this business flow?
- What significant events occur?
- In what broad sequence?
- Who causes each event?
- What decisions are made?
- Which business rules apply?
- What information is required?
- Which exceptions occur?
- Which systems are involved?
- Where are the Hot Spots?
- Where does ownership change?
- Which business concepts have emerged?
- Which domain boundaries require further investigation?
- What Data Product opportunities exist?
- What AI or automation opportunities exist?
- What requires further discovery?

---

# References

Brandolini, A. (2016) *Introducing EventStorming: An Act of Deliberate Collective Learning*. Leanpub. Available at: https://leanpub.com/introducing_eventstorming (Accessed: 10 August 2026).

Brandolini, A. (n.d.a) *EventStorming*. Available at: https://www.eventstorming.com/ (Accessed: 10 August 2026).

Brandolini, A. (n.d.b) *Introducing EventStorming*. EventStorming. Available at: https://www.eventstorming.com/book/ (Accessed: 10 August 2026).

Evans, E. (2004) *Domain-Driven Design: Tackling Complexity in the Heart of Software*. Boston, MA: Addison-Wesley.

Rayner, P. (2024) *The EventStorming Handbook: Unlocking Creativity, Collaboration, and Communication for Your Teams*. Leanpub. Available at: https://leanpub.com/eventstorming_handbook (Accessed: 10 August 2026).