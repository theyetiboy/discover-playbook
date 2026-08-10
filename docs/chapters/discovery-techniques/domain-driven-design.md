---
title: "Domain-Driven Design"
version: "1.0"
author: "Steve Tarry"
technique: "Discovery Technique"
---

# Domain-Driven Design

## Purpose

Domain-Driven Design (DDD) provides a structured approach for understanding complex business domains and creating models that reflect how the business itself understands those domains.

Originally developed as an approach to software design, DDD places particular emphasis on developing deep domain knowledge, collaborating with domain experts and creating a shared language that connects business understanding with solution design (Evans, 2004).

Within DISCOVER, Domain-Driven Design is used primarily as a **discovery and knowledge-modelling technique**.

It helps practitioners:

- Understand complex business domains
- Identify important business concepts
- Establish shared terminology
- Identify domain boundaries
- Understand relationships between business areas
- Discover business rules
- Identify important business events
- Support ontology development
- Define appropriate Data Product boundaries
- Improve the context available to analytics and AI

DISCOVER does not require practitioners to adopt every technical or software-design pattern associated with DDD.

Instead, it selectively applies DDD concepts that improve business understanding.

---

# Why This Technique Matters

Large organisations rarely operate with one simple, universally agreed model of the business.

Different functions may use:

- Different terminology
- Different definitions
- Different business rules
- Different data
- Different measures
- Different systems

The same word may legitimately mean different things in different parts of the organisation.

For example:

```text
Sales
Customer = Organisation purchasing or licensing a product

Finance
Customer = Legal entity responsible for payment

Marketing
Customer = Individual or organisation targeted by marketing activity
```

Trying to create one definition without understanding these contexts can create further ambiguity.

DDD addresses this complexity by recognising that models and terminology exist within defined boundaries known as **Bounded Contexts** (Evans, 2015).

Rather than forcing one enterprise-wide model onto every business area, discovery should first understand where different meanings legitimately exist.

---

# When to Use Domain-Driven Design

DDD techniques are particularly useful when:

- Entering a complex business domain
- Terminology differs between teams
- Business rules are difficult to understand
- Multiple systems represent similar concepts differently
- An Enterprise Ontology is being developed
- Data Products cross organisational boundaries
- Business concepts have ambiguous definitions
- Legacy systems influence business terminology
- Different teams calculate similar metrics differently
- AI capabilities need access to business context
- New platforms are being designed
- Organisational knowledge is fragmented

DDD is particularly valuable where complexity arises from the **business domain itself**, rather than simply from technology.

---

# Core DDD Concepts Used by DISCOVER

DISCOVER primarily uses the following DDD concepts:

1. Domain
2. Subdomain
3. Domain Expert
4. Ubiquitous Language
5. Bounded Context
6. Context Mapping
7. Entities
8. Value Objects
9. Aggregates
10. Domain Events

These concepts help transform informal discovery knowledge into structured business models.

---

# Domain

A **Domain** represents the area of knowledge or activity that the organisation operates within.

Examples might include:

```text
Finance

Marketing

Sales

Content

Rights

Production

Distribution
```

Domains are not necessarily the same as organisational departments.

A domain represents an area of business knowledge and responsibility.

---

# Subdomains

Large domains can often be decomposed into smaller areas of business knowledge.

For example:

```text
Finance
│
├── Financial Planning
├── Revenue Management
├── Financial Reporting
├── Treasury
└── Financial Control
```

Or:

```text
Marketing
│
├── Audience Management
├── Campaign Management
├── Brand Management
├── Marketing Performance
└── Customer Engagement
```

DDD distinguishes between different types of subdomain according to their importance to the organisation (Evans, 2015).

---

# Core Domain

The Core Domain represents business knowledge or capability that provides significant differentiation or strategic value.

Examples might include:

```text
Content Rights Management

Content Monetisation

Audience Intelligence

Revenue Optimisation
```

Whether something is genuinely a Core Domain depends on the organisation's strategy.

The purpose of discovery is to determine this rather than assume it.

---

# Supporting Subdomain

A Supporting Subdomain contributes to the organisation's operation but does not necessarily provide strategic differentiation.

Examples might include:

```text
Supplier Management

Expense Management

Document Management
```

These capabilities remain important but may justify a different investment strategy from Core Domains.

---

# Generic Subdomain

A Generic Subdomain represents functionality required by many organisations and for which established external solutions commonly exist.

Examples might include:

```text
Payroll

Authentication

Email

Commodity Accounting Functions
```

Understanding these distinctions can support later decisions about:

- Investment
- Build vs Buy
- Product ownership
- Technology strategy
- Roadmap prioritisation

---

# Domain Experts

DDD relies heavily on collaboration with people who understand the domain deeply.

These Domain Experts may include:

- Business leaders
- Operational users
- Analysts
- Subject Matter Experts
- Finance specialists
- Legal specialists
- Product specialists

Their expertise often includes knowledge that is:

- Undocumented
- Embedded within processes
- Expressed through specialist language
- Built through experience
- Difficult to infer from systems or data alone

Discovery should therefore involve direct collaboration with Domain Experts rather than relying solely on documentation.

---

# Ubiquitous Language

One of the central concepts within DDD is **Ubiquitous Language**.

The objective is to create a shared language used consistently by domain experts and those designing solutions within a particular model or context (Evans, 2004; Evans, 2015).

Within DISCOVER, Ubiquitous Language connects directly to the:

- Business Glossary
- Enterprise Ontology
- KPI Catalogue
- Data Catalogue
- Data Products
- Semantic Layer
- AI Knowledge Model

For example, a Finance domain might establish clear meanings for:

```text
Revenue

Recognised Revenue

Forecast

Actual

Accrual

Royalty

Margin
```

The objective is not simply to record definitions.

The objective is for participants to **use the agreed terminology consistently when discussing the domain**.

---

# Bounded Context

A **Bounded Context** defines the boundary within which a particular domain model and language apply (Evans, 2015).

This is important because concepts may have different meanings in different contexts.

For example:

```text
                 CUSTOMER

        ┌────────────┼────────────┐
        │            │            │
      SALES       FINANCE      MARKETING
        │            │            │
 Commercial      Billing       Audience
Relationship     Entity        Relationship
```

None of these definitions is necessarily incorrect.

They may represent different models of Customer used for different purposes.

The role of discovery is therefore to understand:

- Where each definition applies
- Why the definition exists
- Who owns it
- How the contexts interact
- How information moves between them

---

# Identifying Bounded Contexts

Potential boundaries may become visible when:

- Terminology changes meaning
- Business rules differ
- Ownership changes
- Different teams control the information
- Different processes apply
- Different systems maintain separate models
- Different lifecycle rules exist

Useful questions include:

- Where does this definition apply?
- Does another team understand this differently?
- Who owns the concept here?
- Where do the rules change?
- At what point does responsibility transfer?
- Does another system represent this differently?

Boundaries should emerge from understanding the business domain rather than being automatically copied from the organisation chart or application architecture.

---

# Context Mapping

Once Bounded Contexts have been identified, DDD encourages explicit modelling of the relationships between them (Evans, 2015).

Within DISCOVER, a **Context Map** provides a high-level view of how business domains interact.

For example:

```text
Sales
  │
  │ Contract / Customer
  ▼
Rights
  │
  │ Rights Availability
  ▼
Distribution
  │
  │ Sales Activity
  ▼
Finance
  │
  │ Revenue / Actuals
  ▼
Reporting
```

A Context Map helps reveal:

- Domain dependencies
- Information handovers
- Ownership boundaries
- Integration requirements
- Semantic differences
- Data Product opportunities

---

# Entities

An **Entity** represents something whose identity remains important throughout its lifecycle (Evans, 2015).

Examples include:

```text
Customer

Programme

Contract

Campaign

Invoice

Rights Agreement
```

A Programme may change:

```text
Title
Status
Metadata
Distribution Status
```

but still represent the same Programme.

Identity therefore matters.

---

# Value Objects

A **Value Object** describes something primarily through its characteristics rather than through a persistent identity (Evans, 2015).

Possible business examples include:

```text
Money

Date Range

Address

Currency Amount

Territory Code
```

Within DISCOVER, distinguishing Entities from Value Objects can help clarify conceptual models and ontology structures.

The distinction should only be introduced where it improves understanding.

---

# Aggregates

DDD uses an **Aggregate** to group related domain objects that should be treated as a consistent unit for particular business operations (Evans, 2015).

For discovery purposes, Aggregates can help identify concepts that naturally belong together.

For example:

```text
Contract
│
├── Contract Party
├── Contract Term
├── Rights Grant
└── Territory
```

This may reveal important business ownership and consistency boundaries.

Detailed Aggregate design normally belongs later in solution design rather than early business discovery.

---

# Domain Events

A Domain Event represents something meaningful that has happened within the business domain.

Examples might include:

```text
Contract Signed

Rights Granted

Programme Commissioned

Campaign Launched

Invoice Issued

Payment Received

Revenue Recognised
```

Events are particularly useful during discovery because stakeholders often find it easier to describe **what happens** than to describe abstract business models.

Domain Events can therefore provide a bridge between:

- Process modelling
- Event Storming
- Ontology modelling
- Data modelling
- Integration design
- AI workflow design

---

# Generic Discovery Questions

## Understanding the Domain

- What business area are we trying to understand?
- What outcomes does this domain deliver?
- What specialist knowledge exists here?
- Which areas are particularly complex?
- Which parts differentiate the organisation?

---

## Understanding Language

- What terminology is unique to this domain?
- Which words are particularly important?
- Which terms regularly cause confusion?
- Do other teams use these terms differently?
- Which acronyms would a newcomer need to understand?

---

## Understanding Boundaries

- Where does this team's responsibility begin?
- Where does it end?
- When does ownership transfer to another team?
- Which concepts change meaning across that boundary?
- Which rules apply only within this area?

---

## Understanding Concepts

- What are the important business things you work with?
- Which have a unique identity?
- How do they relate?
- Which concepts exist inside other concepts?
- Which concepts have their own lifecycle?

---

## Understanding Rules

- What rules govern this domain?
- Which rules determine whether an action can occur?
- Which rules are regulatory?
- Which rules are undocumented?
- Where are exceptions allowed?

---

## Understanding Events

- What important events happen within this domain?
- What triggers them?
- What happens afterwards?
- Which teams need to know?
- Which systems record those events?

---

## Understanding Relationships

- Which other domains do you depend upon?
- What information do you receive?
- What information do you provide?
- Where do semantic misunderstandings occur?
- Which handovers regularly cause problems?

---

# DDD Discovery Workshop

A lightweight DDD discovery workshop might follow this structure.

| Stage | Activity |
|-------|----------|
| 1 | Define the domain |
| 2 | Identify Domain Experts |
| 3 | Identify important terminology |
| 4 | Capture business concepts |
| 5 | Identify business rules |
| 6 | Identify major business events |
| 7 | Identify possible domain boundaries |
| 8 | Identify relationships between domains |
| 9 | Capture semantic conflicts |
| 10 | Validate findings |

The workshop should remain business focused.

Avoid introducing unnecessary software architecture terminology where it does not help participants.

---

# Finance Example

## Discovery Objective

Understand the Finance domain and identify important terminology, concepts, rules and boundaries.

An initial domain model might expose:

```text
Finance
│
├── Financial Planning
│
├── Revenue Management
│
├── Financial Reporting
│
├── Treasury
│
└── Financial Control
```

Further discovery may reveal different contexts.

For example:

```text
Sales Context

Contract
Customer
Booked Value
Sales Forecast

        │
        ▼

Finance Context

Contract
Billing Customer
Recognised Revenue
Financial Forecast
Actual

        │
        ▼

Reporting Context

Revenue KPI
Forecast Variance
P&L
Management Reporting
```

### Example Questions

- What does Revenue mean within Finance?
- When does booked value become recognised revenue?
- Does Sales use the same definition?
- Which rules determine recognition?
- Who owns those rules?
- What constitutes an Actual?
- When does a Forecast become an Actual?
- Where does contract information enter Finance?
- Which important business events affect revenue?
- Where does Finance responsibility begin and end?

### Potential Domain Events

```text
Contract Signed

Invoice Raised

Revenue Recognised

Forecast Updated

Payment Received

Period Closed
```

### Potential Findings

Discovery may reveal:

- Sales and Finance use different models of Revenue.
- Customer identity differs between CRM and Finance.
- Revenue Recognition contains specialist business rules.
- Forecast definitions vary between teams.
- Reporting combines concepts originating from several contexts.

### Potential Outputs

- Finance Ubiquitous Language
- Finance Bounded Contexts
- Context Map
- Revenue Domain Model
- Finance Business Glossary
- Revenue Ontology Concepts
- Business Rules Catalogue

---

# Marketing Example

## Discovery Objective

Understand how Marketing models campaigns, audiences and performance.

Possible contexts might include:

```text
Campaign Planning
        │
        ▼
Campaign Delivery
        │
        ▼
Audience Management
        │
        ▼
Performance Measurement
```

The concept of **Audience** may differ between these contexts.

For example:

```text
Planning Context

Target Audience

        │
        ▼

Activation Context

Addressable Audience

        │
        ▼

Measurement Context

Reached Audience
```

### Example Questions

- What constitutes a Campaign?
- When does a Campaign begin and end?
- What is an Audience?
- What is a Segment?
- Does Audience mean the same thing across platforms?
- What constitutes Engagement?
- What constitutes Conversion?
- Which business events occur during the campaign lifecycle?
- Where does campaign ownership transfer?
- Which concepts come from external marketing platforms?

### Potential Domain Events

```text
Campaign Created

Campaign Approved

Campaign Launched

Audience Selected

Impression Delivered

Conversion Recorded

Campaign Completed
```

### Potential Findings

Discovery may reveal:

- Different platforms use different definitions of Engagement.
- Campaign identifiers differ across systems.
- Audience terminology changes between planning and measurement.
- Attribution has multiple domain-specific interpretations.
- Marketing and Finance use different models of campaign cost and return.

### Potential Outputs

- Marketing Ubiquitous Language
- Marketing Context Map
- Campaign Domain Model
- Audience Ontology
- Marketing Business Glossary
- Business Rules Catalogue

---

# Connecting DDD to the Business Glossary

DDD and Business Glossary discovery strongly reinforce each other.

```text
Domain Experts
      │
      ▼
Business Language
      │
      ▼
Ubiquitous Language
      │
      ▼
Business Glossary
```

However, the glossary should retain context.

Instead of forcing:

```text
Customer = One Enterprise Definition
```

DDD may reveal:

```text
Sales.Customer

Finance.Customer

Marketing.Customer
```

These concepts can then be explicitly related through the Enterprise Ontology.

---

# Connecting DDD to Ontology Discovery

DDD helps establish the **meaning and boundaries** of business concepts.

Ontology modelling helps represent the **relationships between those concepts**.

For example:

```text
Sales Context

Customer
   │
   └── SIGNS → Contract


Rights Context

Contract
   │
   └── GRANTS → Rights


Content Context

Rights
   │
   └── APPLY TO → Programme


Finance Context

Contract
   │
   └── GENERATES → Revenue
```

DDD therefore provides important context that helps prevent an Enterprise Ontology from becoming an oversimplified global model.

---

# Connecting DDD to Data Products

DDD can help determine appropriate Data Product boundaries.

For example:

```text
Rights Domain
      │
      └── Rights Availability Data Product


Finance Domain
      │
      └── Revenue Performance Data Product


Marketing Domain
      │
      └── Campaign Performance Data Product
```

Cross-domain products can then consume clearly defined information products from multiple domains rather than recreating domain logic independently.

---

# Connecting DDD to AI

AI systems frequently operate across large bodies of organisational knowledge.

Without domain context, terms can become ambiguous.

DDD concepts can help provide AI systems with context such as:

```text
Term
+
Domain
+
Definition
+
Relationships
+
Business Rules
```

For example:

```text
"Revenue"

Context = Finance

Definition = Recognised Revenue

Rules = Finance Revenue Recognition Rules
```

This can provide richer semantic context for:

- Enterprise Search
- Retrieval-Augmented Generation
- Knowledge Assistants
- Conversational Analytics
- AI Agents

DDD does not itself solve AI accuracy or governance problems, but its emphasis on explicit context and shared language can strengthen the knowledge foundation supplied to AI systems.

---

# Connecting DDD to POPIT-V

DDD can inform every POPIT-V perspective.

## People

- Who are the Domain Experts?
- Who owns business definitions?
- Who understands specialist rules?

## Organisation

- What domains exist?
- Where do responsibilities sit?
- Which domains provide strategic differentiation?

## Process

- Which events occur?
- Which commands or decisions trigger them?
- How does work move between contexts?

## Information

- What concepts exist?
- What terminology is used?
- What relationships and rules apply?

## Technology

- Which systems currently represent each domain?
- Do system boundaries align with business boundaries?

## Value

- Which domains provide strategic value?
- Where should investment be concentrated?

---

# Common Pitfalls

## Treating DDD as a Software-Only Technique

DISCOVER uses DDD primarily to improve business understanding.

Do not begin discussing code, microservices or technical implementation unless it is relevant to the discovery objective.

---

## Assuming Department = Domain

Organisation charts can provide clues, but business domain boundaries should emerge from:

- Language
- Responsibility
- Rules
- Knowledge
- Behaviour

---

## Creating One Enterprise Model Too Early

Do not force every team to agree on one definition before understanding why differences exist.

Identify context first.

Standardise only where it creates genuine value.

---

## Using Technical Language with Business Stakeholders

Avoid opening a workshop with:

```text
Entities

Aggregates

Repositories

Bounded Contexts
```

Instead ask:

```text
What are the important things?

What happens to them?

What rules apply?

Who owns them?

Where does their meaning change?
```

The modelling terminology can be applied afterwards.

---

## Modelling Everything

DDD should focus attention on meaningful business complexity.

Not every reference table or operational field needs sophisticated domain modelling.

---

## Letting Existing Systems Define the Domain

A legacy application may contain terminology and boundaries created by technical decisions made many years ago.

Treat the system as evidence.

Do not automatically treat it as the correct model of the business.

---

# What Good Looks Like

Effective DDD discovery should result in:

- Identified business domains
- Relevant subdomains
- Identified Domain Experts
- Shared business language
- Clear domain terminology
- Candidate Bounded Contexts
- Documented relationships between contexts
- Important business concepts
- Important business rules
- Major Domain Events
- Identified semantic conflicts
- Inputs into ontology development
- Inputs into Data Product design

---

# Discovery Outputs

DDD discovery should contribute to:

- Business Glossary
- Domain Map
- Context Map
- Domain Model
- Enterprise Ontology
- Business Rules Catalogue
- Event Catalogue
- Data Product Boundaries
- Data Ownership
- Semantic Layer Requirements
- AI Knowledge Requirements

---

# Related DISCOVER Techniques

DDD works particularly well alongside:

- Business Capability Mapping
- Business Glossary
- Event Storming
- Ontology Discovery
- Process Modelling
- Stakeholder Mapping
- Data Product Design

A typical sequence might be:

```text
Capability Mapping
        │
        ▼
Domain Discovery
        │
        ▼
Business Glossary
        │
        ▼
Event Storming
        │
        ▼
Bounded Contexts
        │
        ▼
Ontology Discovery
        │
        ▼
Data Products
```

The sequence is not mandatory.

DISCOVER techniques should be selected according to the needs of the engagement.

---

# Recommended Discovery Questions – Quick Reference

Before concluding DDD discovery, ensure you can answer:

- What business domain are we exploring?
- Who are the Domain Experts?
- What terminology is important?
- What do the key terms mean?
- Where does terminology change meaning?
- What are the major business concepts?
- Which rules govern those concepts?
- What events occur?
- Where do responsibilities change?
- What are the likely Bounded Contexts?
- How do those contexts interact?
- What information crosses those boundaries?
- Which domains should own particular Data Products?
- What should feed the Enterprise Ontology?

---

# References

Evans, E. (2004) *Domain-Driven Design: Tackling Complexity in the Heart of Software*. Boston, MA: Addison-Wesley.

Evans, E. (2015) *Domain-Driven Design Reference: Definitions and Pattern Summaries*. Domain Language. Available at: https://www.domainlanguage.com/wp-content/uploads/2016/05/DDD_Reference_2015-03.pdf (Accessed: 10 August 2026).

Evans, E. (n.d.) *DDD Reference*. Domain Language. Available at: https://www.domainlanguage.com/ddd/reference/ (Accessed: 10 August 2026).

Evans, E. (n.d.) *DDD Resources*. Domain Language. Available at: https://www.domainlanguage.com/ddd/ (Accessed: 10 August 2026).

Fowler, M. (2014) 'Bounded Context'. *martinfowler.com*, 15 January. Available at: https://martinfowler.com/bliki/BoundedContext.html (Accessed: 10 August 2026).