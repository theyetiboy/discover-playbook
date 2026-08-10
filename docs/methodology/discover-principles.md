---
title: "DISCOVER Principles"
version: "1.0"
author: "Steve Tarry"
methodology: "DISCOVER"
---

# DISCOVER Principles

## Purpose

The DISCOVER Principles define the behaviours and decision rules that guide how discovery should be performed.

The DISCOVER Framework provides the stages:

```text
Define
Investigate
Study
Capture
Organise
Validate
Evaluate
Roadmap
```

The principles describe **how practitioners should think and behave while moving through those stages**.

They are intended to prevent discovery becoming:

- Technology led
- Solution led
- Documentation heavy
- Siloed
- Assumption driven
- Disconnected from business outcomes
- Focused on outputs rather than value

The principles should be applied across all DISCOVER engagements regardless of business domain.

---

# The DISCOVER Principles

```text
1.  Business Before Technology

2.  Start With Outcomes

3.  Decisions Drive Data

4.  Model the Business, Not the Systems

5.  Understand People in Context

6.  Evidence Over Assumption

7.  Create Shared Understanding

8.  Capture Knowledge Once, Reuse It

9.  Connect Everything

10. Explore Before You Converge

11. Remain Solution Neutral

12. Validate Continuously

13. Design Governance In

14. Every Recommendation Must Deliver Value
```

Together these principles provide the foundation for how DISCOVER should be practised.

---

# 1. Business Before Technology

## Principle

> **Understand the business before discussing the technology.**

Technology should enable business capability.

It should not define the problem.

Discovery should therefore begin with:

```text
Business Strategy

Business Outcomes

Business Capabilities

Users

Processes

Decisions

Information

Pain Points

Value
```

before moving towards:

```text
Applications

Platforms

Architecture

Data Pipelines

Cloud Services

AI

Vendor Products
```

---

## Why It Matters

Technology-led discovery can cause the solution to be predetermined before the problem is understood.

Examples include:

```text
"We need a dashboard."

"We need a Data Lake."

"We need GenAI."

"We need a Knowledge Graph."

"We need to migrate this platform."

"We need a new CRM."
```

Each of these statements should trigger the question:

> **Why?**

Continue until the underlying business need becomes clear.

For example:

```text
"We need a dashboard."

        │
        ▼

Why?

        │
        ▼

"We can't understand revenue performance."

        │
        ▼

Why?

        │
        ▼

"Actual and forecast revenue are difficult to reconcile."

        │
        ▼

Why?

        │
        ▼

"Contract, forecast and actual revenue data
exist in different systems and use
different business rules."
```

The original dashboard request is now understood in a much richer context.

---

## DISCOVER Behaviour

Ask:

- What business problem are we solving?
- Which outcome needs to improve?
- Who experiences the problem?
- What decision is difficult today?
- What capability is affected?
- What evidence demonstrates the problem?

Only then ask:

> **What technology, if any, could help?**

---

# 2. Start With Outcomes

## Principle

> **Start with the outcome the organisation or user needs to achieve.**

Discovery should focus on outcomes rather than outputs.

For example:

```text
OUTPUT

Build a Revenue Dashboard
```

versus:

```text
OUTCOME

Enable Finance leaders to identify
revenue variance early enough
to take corrective action.
```

The outcome leaves room for discovery.

The output assumes the solution.

IIBA defines business analysis around identifying needs and recommending solutions that deliver value to stakeholders (IIBA, n.d.a).

DISCOVER applies the same outcome-oriented philosophy.

---

## Business Outcomes

Potential outcomes might include:

```text
Increase Revenue

Reduce Cost

Improve Forecast Accuracy

Reduce Reporting Time

Improve Customer Experience

Increase Content Sales

Reduce Process Failure

Improve Regulatory Compliance

Improve Decision Quality

Increase Operational Efficiency
```

Outcomes provide a reference point throughout discovery.

---

## DISCOVER Behaviour

Continually ask:

```text
What are we trying to improve?

For whom?

Why does it matter?

How will we know it has improved?
```

If those questions cannot be answered, further discovery is required.

---

# 3. Decisions Drive Data

## Principle

> **Understand the decision before defining the data requirement.**

Organisations frequently begin Data & Analytics conversations by asking:

```text
What data do we have?
```

DISCOVER encourages a different starting point:

```text
What decision needs to be made?
```

Then:

```text
Decision
    │
    ▼
Information Required
    │
    ▼
Business Concepts
    │
    ▼
Business Rules
    │
    ▼
Data Required
    │
    ▼
Data Product
```

---

## Example

A Finance Director may need to decide:

```text
"Do we need to revise the current revenue forecast?"
```

That decision may require:

```text
Actual Revenue

Forecast Revenue

Contracted Revenue

Pipeline

Variance

Historical Performance

Territory

Currency
```

Only after understanding that information should the underlying datasets be designed.

---

## Why It Matters

Starting with available data often produces:

```text
Data Products looking for users.
```

Starting with decisions helps produce:

```text
Data Products designed to support action.
```

---

## DISCOVER Behaviour

For every significant analytical requirement ask:

```text
Who is making the decision?

What decision are they making?

When do they make it?

What information do they require?

What happens after the decision?

What happens if the information is wrong or late?
```

---

# 4. Model the Business, Not the Systems

## Principle

> **Business meaning should exist independently of its current technical implementation.**

Existing technology provides useful evidence about the organisation.

It should not automatically define the organisation.

For example:

```text
Poor Starting Point

Salesforce Account
Oracle Contract
Spreadsheet Forecast
```

Instead identify the underlying business concepts:

```text
Customer

Contract

Forecast
```

The systems can then be mapped against those concepts.

---

## Why It Matters

Systems change.

Business concepts frequently survive those changes.

For example:

```text
Customer

Contract

Programme

Rights

Revenue

Campaign

Territory
```

may exist for decades while the applications used to manage them change repeatedly.

Modelling the business independently of systems therefore creates a more stable foundation for:

- Enterprise Architecture
- Data Products
- Ontologies
- Semantic Layers
- Integration
- Analytics
- AI

---

## DISCOVER Behaviour

Ask:

```text
What is the business concept?

What does it mean?

Who owns it?

What rules govern it?

Where is it represented?
```

rather than:

```text
What tables exist in this application?
```

Technical discovery follows business discovery.

---

# 5. Understand People in Context

## Principle

> **Understand what people are trying to achieve, not simply what they ask for.**

GOV.UK's Service Standard emphasises developing a deep understanding of users and the problems they are trying to solve, including the wider context surrounding their experience (Government Digital Service, 2019).

DISCOVER applies that principle to enterprise discovery.

Users may include:

```text
Customers

Employees

Analysts

Executives

Finance Teams

Sales Teams

Operational Users

Partners

Suppliers
```

---

## Stated Need vs Underlying Need

A stakeholder may say:

```text
"I need another report."
```

Further investigation may reveal:

```text
"I need to know which contracts
are likely to miss forecast."
```

The second statement describes the actual information need.

---

## Observe Work

Where appropriate, ask:

> **Can you show me how you actually do this?**

Observation can expose:

- Spreadsheets
- Manual workarounds
- Copy and paste
- Reconciliation
- Email approvals
- Informal knowledge
- System switching
- Undocumented business rules

GDS user-research guidance similarly recommends understanding what users are trying to achieve, how they currently do it and the problems they experience (Government Digital Service, 2016).

---

## DISCOVER Behaviour

Understand:

```text
Goals

Responsibilities

Activities

Decisions

Information Needs

Pain Points

Workarounds

Constraints

Success Measures
```

Do not reduce stakeholders to requirements providers.

They are participants in the business system being discovered.

---

# 6. Evidence Over Assumption

## Principle

> **Distinguish what is known from what is believed.**

Discovery frequently contains statements such as:

```text
"Everyone uses this."

"This always happens."

"The data is bad."

"Finance owns that."

"Nobody uses this report."

"We can't automate this."
```

These may be correct.

They may also be assumptions.

DISCOVER should make the distinction visible.

---

# Evidence Classification

Use categories such as:

| Classification | Meaning |
|---|---|
| Fact | Supported by evidence |
| Observation | Directly observed during discovery |
| Stakeholder View | Perspective expressed by a stakeholder |
| Assumption | Believed to be true but not validated |
| Hypothesis | Explanation that can be tested |
| Finding | Conclusion supported by discovery evidence |

---

## Example

Instead of:

```text
FINDING

Nobody uses Report X.
```

capture:

```text
STAKEHOLDER VIEW

Three interviewees stated that
they do not use Report X.


EVIDENCE REQUIRED

Usage analytics.


VALIDATED FINDING

Report X received 14 views
during the previous six months.
```

This creates a much stronger basis for decision-making.

---

## DISCOVER Behaviour

Ask:

```text
How do we know?

What evidence supports this?

Who else should we ask?

Can we observe it?

Can we measure it?

Can we validate it with data?
```

---

# 7. Create Shared Understanding

## Principle

> **Discovery should create a common understanding of the business, not separate interpretations held by individual teams.**

Large organisations frequently contain multiple perspectives.

For example:

```text
Sales
   │
   └── Customer


Finance
   │
   └── Customer


Marketing
   │
   └── Customer
```

These perspectives may legitimately differ.

The objective is not necessarily to force one definition.

The objective is to make the differences **explicit and understood**.

---

## Shared Understanding Comes From Collaboration

DISCOVER therefore favours collaborative techniques such as:

- Workshops
- Event Storming
- Capability Mapping
- Process Modelling
- Business Glossary sessions
- Ontology Discovery
- Playback Sessions

The Design Council similarly emphasises working with people affected by the problem and using divergent and convergent approaches to build understanding and develop responses (Design Council, n.d.).

---

## DISCOVER Behaviour

Create situations where stakeholders can:

```text
See

Challenge

Discuss

Refine

Agree

Disagree Explicitly

Validate
```

A useful discovery outcome is often:

> **"We didn't realise the other team understood it that way."**

That is new organisational knowledge.

---

# 8. Capture Knowledge Once, Reuse It

## Principle

> **Knowledge discovered once should become reusable organisational knowledge.**

Discovery requires significant stakeholder time.

The same questions should not need to be asked repeatedly by different projects.

For example:

```text
What is Revenue?

Who owns Revenue?

How is Revenue calculated?

Which systems contain Revenue?

Which processes create Revenue?
```

If this has already been discovered and validated, it should be available for reuse.

---

# Reusable Knowledge

DISCOVER captures knowledge into structured artefacts such as:

```text
Business Glossary

Capability Catalogue

Process Catalogue

Ontology

Data Catalogue

KPI Catalogue

Business Rules

Stakeholder Register

RACI

Data Product Catalogue
```

These should form an increasingly rich organisational knowledge base.

---

## From Project Documentation to Organisational Knowledge

Traditional discovery may produce:

```text
Project Folder

      │
      ▼

Workshop Notes

      │
      ▼

PowerPoint

      │
      ▼

Archive
```

DISCOVER aims for:

```text
Discovery
    │
    ▼
Structured Knowledge
    │
    ▼
Shared Repository
    │
    ▼
Future Discovery
    │
    ▼
Enrichment
```

Each discovery engagement should increase organisational understanding.

---

## DISCOVER Behaviour

Before asking a stakeholder:

> What does this term mean?

first ask:

> Do we already have a validated definition?

Reuse where possible.

Validate where necessary.

Extend rather than recreate.

---

# 9. Connect Everything

## Principle

> **Discovery artefacts should not exist as isolated documents.**

The value of DISCOVER increases when relationships between artefacts are maintained.

For example:

```text
Business Strategy
      │
      ▼
Capability
      │
      ▼
Process
      │
      ▼
Decision
      │
      ▼
Information
      │
      ▼
KPI
      │
      ▼
Data
      │
      ▼
Data Product
      │
      ▼
Action
      │
      ▼
Value
```

This is the DISCOVER Golden Thread.

---

# Connected Knowledge

A Business Capability should connect to:

```text
Owner

Processes

Information

Systems

KPIs

Data Products

Opportunities
```

A KPI should connect to:

```text
Business Definition

Owner

Business Objective

Capability

Process

Data

Reports

Data Products
```

A Data Product should connect to:

```text
User

Decision

Business Outcome

Capabilities

Information

Data

Technology

Value
```

---

## Why It Matters

Without traceability, organisations can accumulate artefacts without understanding how they relate.

For example:

```text
500 KPIs

200 Reports

100 Datasets

50 Systems
```

may provide little insight unless the organisation understands:

```text
Why they exist.

Who uses them.

What decisions they support.

What value they create.
```

---

## DISCOVER Behaviour

Whenever something important is captured ask:

> **What does this connect to?**

---

# 10. Explore Before You Converge

## Principle

> **Do not select the answer before sufficiently understanding the problem.**

Discovery requires both:

```text
Divergence
```

and:

```text
Convergence
```

The Design Council's Double Diamond explicitly describes exploring a problem widely or deeply before taking focused action (Design Council, n.d.).

---

# Divergence

During exploration:

```text
Ask questions

Gather perspectives

Explore processes

Identify pain points

Understand exceptions

Identify opportunities

Challenge assumptions
```

Do not eliminate possibilities too quickly.

---

# Convergence

Once sufficient understanding exists:

```text
Organise findings

Validate evidence

Identify themes

Evaluate opportunities

Prioritise

Recommend
```

---

## DISCOVER Behaviour

Avoid:

```text
Stakeholder Request
      │
      ▼
Immediate Solution
```

Prefer:

```text
Stakeholder Request
      │
      ▼
Explore
      │
      ▼
Understand
      │
      ▼
Validate
      │
      ▼
Evaluate Options
      │
      ▼
Recommend
```

---

# 11. Remain Solution Neutral

## Principle

> **The best solution may not be technology.**

DISCOVER should remain neutral about the form of the eventual response.

A problem may require:

```text
Process Change

Policy Change

Clear Ownership

Business Rule

Training

Data Quality Improvement

System Integration

Data Product

Analytics

Automation

AI

New Technology

No Change
```

---

# Avoid Technology Bias

For example:

```text
PROBLEM

Users cannot find the correct definition
of important business measures.
```

Possible responses include:

```text
Better Documentation

Business Glossary

Semantic Layer

Metadata Catalogue

Search

Knowledge Assistant
```

AI may eventually be appropriate.

It should not automatically be the first answer.

---

## Simplest Effective Response

Where several options create similar value, prefer the response that achieves the outcome with proportionate:

```text
Complexity

Cost

Risk

Time

Operational Burden
```

The goal is not technological sophistication.

The goal is business improvement.

---

# 12. Validate Continuously

## Principle

> **Validation is an activity throughout discovery, not merely a final stage.**

Although DISCOVER contains a dedicated **Validate** stage, validation should occur continuously.

For example:

```text
Interview
   │
   ▼
Capture Finding
   │
   ▼
Check With Another Stakeholder
   │
   ▼
Update Understanding
```

or:

```text
Process Workshop
   │
   ▼
Draft Process
   │
   ▼
Playback
   │
   ▼
Correct
```

---

# Why It Matters

Without continuous validation:

```text
Small Misunderstanding

        │
        ▼

Embedded Assumption

        │
        ▼

Incorrect Model

        │
        ▼

Incorrect Requirement

        │
        ▼

Incorrect Solution
```

IIBA describes validation as assessing whether a deliverable or requirement is suitable for its intended use and supports expected benefits (IIBA, n.d.b).

---

## DISCOVER Behaviour

Use:

```text
Playback

Peer Review

Stakeholder Review

Data Validation

Process Walkthrough

Prototype

Experiment

Evidence
```

to progressively increase confidence.

---

# 13. Design Governance In

## Principle

> **Ownership, quality, risk and governance should be considered during discovery rather than added after delivery.**

For every important business concept ask:

```text
Who owns it?

Who maintains it?

Who approves changes?

How is quality measured?

Who has access?

What rules apply?
```

For a Data Product ask:

```text
Who owns the product?

Who owns the data?

Who defines quality?

Who supports it?

Who can access it?

How is change governed?
```

---

# Governance Should Be Proportionate

Governance does not mean adding unnecessary process.

Controls should reflect:

```text
Business Criticality

Risk

Regulation

Sensitivity

Financial Impact

Decision Impact
```

A locally used operational measure may require lightweight governance.

A statutory financial metric may require significantly stronger controls.

---

# AI Governance

The same principle applies to AI.

AI opportunities should consider from discovery:

- Accountability
- Data suitability
- Privacy
- Security
- Reliability
- Human oversight
- Monitoring
- Potential harm
- Escalation
- Appropriate use

The NIST AI Risk Management Framework structures AI risk management around **Govern, Map, Measure and Manage**, reinforcing that governance and risk management should be integrated throughout the AI lifecycle rather than treated only as a final control (NIST, 2023).

---

## DISCOVER Behaviour

Do not ask only:

> Can we build it?

Also ask:

```text
Should we build it?

Who owns it?

How will we know it works?

How will failure be handled?

What controls are required?
```

---

# 14. Every Recommendation Must Deliver Value

## Principle

> **Every recommendation should be traceable to a meaningful business outcome.**

DISCOVER should not recommend something simply because it is:

```text
Interesting

Modern

Technically Elegant

Popular

Available

Requested by One Stakeholder
```

IIBA defines value as the worth, importance or usefulness of something to a stakeholder within a particular context (IIBA, n.d.b).

DISCOVER therefore expects recommendations to explain:

```text
Problem

        │
        ▼

Opportunity

        │
        ▼

Business Outcome

        │
        ▼

Benefit

        │
        ▼

Measure
```

---

# Types of Value

Value may include:

## Revenue

```text
Increased Sales

Higher Conversion

Improved Monetisation
```

---

## Cost

```text
Reduced Manual Effort

Reduced Technology Cost

Reduced External Spend
```

---

## Time

```text
Faster Reporting

Shorter Process Lead Time

Faster Decisions
```

---

## Quality

```text
Improved Data Quality

Reduced Errors

Improved Forecast Accuracy
```

---

## Risk

```text
Improved Compliance

Reduced Financial Risk

Improved Auditability
```

---

## Customer

```text
Improved Experience

Faster Service

Better Personalisation
```

---

## Strategic

```text
Improved Capability

Competitive Advantage

New Business Model

Improved Organisational Knowledge
```

---

# Measure the Outcome

Where possible define:

```text
Current State

Target State

Measure

Owner

Measurement Frequency
```

Example:

```text
Opportunity

Automated Revenue Reconciliation


Current State

4 days manual reconciliation per month


Target

1 day


Measure

Reconciliation Cycle Time


Benefit

3 days Finance capacity released monthly
```

Value should become measurable where practical.

---

# Applying the Principles Together

The principles are designed to reinforce one another.

Consider a request:

```text
"We need an AI Finance Assistant."
```

Apply the DISCOVER Principles:

```text
Business Before Technology
        │
        ▼
What business problem exists?


Start With Outcomes
        │
        ▼
What outcome should improve?


Understand People in Context
        │
        ▼
Who needs help and what are they doing?


Decisions Drive Data
        │
        ▼
What decisions or activities need support?


Evidence Over Assumption
        │
        ▼
How do we know the problem exists?


Model the Business
        │
        ▼
What Finance concepts and rules matter?


Create Shared Understanding
        │
        ▼
Do stakeholders agree?


Capture Knowledge Once
        │
        ▼
Can Finance knowledge be governed and reused?


Connect Everything
        │
        ▼
What capabilities, processes and data are involved?


Explore Before Converging
        │
        ▼
What options exist?


Remain Solution Neutral
        │
        ▼
Is AI actually the best response?


Validate Continuously
        │
        ▼
Can we test the assumptions?


Design Governance In
        │
        ▼
What controls and ownership are required?


Deliver Value
        │
        ▼
Is the benefit sufficient to justify investment?
```

The result may still be:

```text
AI Finance Assistant
```

But it is now a response to a validated business need rather than a technology looking for a problem.

---

# Principles Across POPIT-V

The DISCOVER Principles apply across all six POPIT-V perspectives.

| POPIT-V | Principle Focus |
|---|---|
| People | Understand users, knowledge, ownership and impact |
| Organisation | Connect discovery to strategy, governance and capability |
| Process | Understand how work actually happens |
| Information | Define meaning, quality, ownership and relationships |
| Technology | Treat technology as an enabler rather than the starting point |
| Value | Ensure recommendations produce meaningful outcomes |

---

# Principles Across the DISCOVER Framework

The emphasis of individual principles may change throughout the eight stages.

| Stage | Key Principle Emphasis |
|---|---|
| Define | Business Before Technology |
| Define | Start With Outcomes |
| Investigate | Understand People in Context |
| Investigate | Evidence Over Assumption |
| Study | Model the Business, Not the Systems |
| Study | Decisions Drive Data |
| Capture | Capture Knowledge Once, Reuse It |
| Organise | Connect Everything |
| Validate | Create Shared Understanding |
| Validate | Validate Continuously |
| Evaluate | Remain Solution Neutral |
| Evaluate | Design Governance In |
| Evaluate | Every Recommendation Must Deliver Value |
| Roadmap | Every Recommendation Must Deliver Value |

These are emphasis points rather than fixed boundaries.

Every principle applies throughout DISCOVER.

---

# Principle Conflicts

Principles may occasionally appear to compete.

For example:

```text
Capture Knowledge Once

vs

Avoid Unnecessary Documentation
```

or:

```text
Validate Continuously

vs

Maintain Discovery Momentum
```

The answer should be proportionate.

DISCOVER is not intended to create bureaucracy.

Ask:

> **What level of effort is appropriate for the value, risk and uncertainty involved?**

The principles are guides for judgement, not rigid rules.

---

# Anti-Patterns

The following behaviours should trigger challenge during DISCOVER.

## Technology First

```text
"We've already selected the platform.
Now let's find the use cases."
```

---

## Output First

```text
"The deliverable needs to be a dashboard."
```

---

## Data First

```text
"Let's expose everything in the database
and see what users do with it."
```

---

## System-Led Modelling

```text
"Our definition of Customer is whatever
the CRM currently contains."
```

---

## Opinion as Fact

```text
"Everyone hates this process."
```

---

## Documentation Without Reuse

```text
"We've defined this before,
but nobody knows where."
```

---

## Artefact Silos

```text
The process map does not connect
to the data model, KPI definitions,
ownership or roadmap.
```

---

## Solution Bias

```text
"The answer has to involve AI."
```

---

## Governance Later

```text
"We'll work out ownership after launch."
```

---

## Value Unknown

```text
"We should build it because
stakeholders asked for it."
```

Each is a signal to return to the DISCOVER Principles.

---

# Practitioner Checklist

Before making a significant recommendation, ask:

- [ ] Have we understood the underlying business problem?
- [ ] Is the desired outcome clear?
- [ ] Do we understand the relevant users?
- [ ] Do we understand the decisions involved?
- [ ] Do we understand the required information?
- [ ] Have we modelled the business independently of existing systems?
- [ ] Is the finding supported by evidence?
- [ ] Have relevant stakeholders validated our understanding?
- [ ] Have important definitions been captured?
- [ ] Can existing organisational knowledge be reused?
- [ ] Are artefacts connected through the Golden Thread?
- [ ] Have we explored alternative responses?
- [ ] Are we remaining solution neutral?
- [ ] Is ownership clear?
- [ ] Have governance and risk been considered?
- [ ] Is the recommendation proportionate?
- [ ] Can the expected value be explained?
- [ ] Can success be measured?

If several answers are:

```text
No
```

then the recommendation may be premature.

---

# The DISCOVER Mindset

The principles can ultimately be summarised as:

```text
Ask before assuming.

Understand before designing.

Observe before modelling.

Model the business before the technology.

Understand the decision before the data.

Capture knowledge rather than documents.

Connect rather than isolate.

Validate rather than presume.

Explore before selecting.

Govern by design.

Recommend only where value exists.
```

---

# Related DISCOVER Methodology

The DISCOVER Principles should be read alongside:

- The DISCOVER Framework
- The Golden Thread
- POPIT-V Overview
- Maturity Model
- Discovery Techniques
- Workshop Playbook
- Data Product Design
- AI Opportunity Discovery
- Prioritisation
- Roadmapping

---

# References

Design Council (n.d.) *Framework for Innovation: Design Council's evolved Double Diamond*. London: Design Council. Available at: https://www.designcouncil.org.uk/our-resources/framework-for-innovation/ (Accessed: 10 August 2026).

Government Digital Service (2016) *User research in discovery*. GOV.UK Service Manual. Available at: https://www.gov.uk/service-manual/user-research/user-research-in-discovery (Accessed: 10 August 2026).

Government Digital Service (2019) *Understand users and their needs*. GOV.UK Service Manual. Available at: https://www.gov.uk/service-manual/service-standard/point-1-understand-user-needs (Accessed: 10 August 2026).

Government Digital Service (n.d.) *How the discovery phase works*. GOV.UK Service Manual. Available at: https://www.gov.uk/service-manual/agile-delivery/how-the-discovery-phase-works (Accessed: 10 August 2026).

International Institute of Business Analysis (IIBA) (n.d.a) *Defining Business Analysis*. The Business Analysis Standard. Available at: https://www.iiba.org/knowledgehub/the-business-analysis-standard/2-understanding-business-analysis/2-1-defining-business-analysis/ (Accessed: 10 August 2026).

International Institute of Business Analysis (IIBA) (n.d.b) *BABOK® Guide Appendix A: Glossary*. Available at: https://www.iiba.org/career-resources/a-business-analysis-professionals-foundation-for-success/babok/glossary/ (Accessed: 10 August 2026).

National Institute of Standards and Technology (NIST) (2023) *Artificial Intelligence Risk Management Framework (AI RMF 1.0)*. NIST AI 100-1. Gaithersburg, MD: U.S. Department of Commerce. Available at: https://www.nist.gov/itl/ai-risk-management-framework (Accessed: 10 August 2026).

---

# Attribution

The **DISCOVER Principles** are original principles developed as part of the DISCOVER Data Product Discovery Playbook.

They draw upon and adapt established practices from Business Analysis, Service Design, Product Management, Business Architecture, Data Management and responsible AI.

External frameworks and standards are referenced where they provide supporting foundations, but the principles and their application within the DISCOVER methodology are original to this playbook.