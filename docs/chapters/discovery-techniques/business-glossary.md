---
title: "Business Glossary"
version: "1.0"
author: "Steve Tarry"
technique: "Discovery Technique"
---

# Business Glossary

## Purpose

A Business Glossary provides a shared and governed vocabulary for the terms used within a business domain.

It captures the meaning of important business concepts in language that can be understood consistently across business, product, data and technology teams.

The International Institute of Business Analysis (IIBA) describes a glossary as a technique for defining key terms relevant to a business domain (IIBA, n.d.).

Within DISCOVER, the Business Glossary provides an important bridge between business discovery and subsequent information modelling, ontology development, data product design and analytics.

It is particularly useful during the **Investigate**, **Capture**, **Organise** and **Validate** stages of the DISCOVER framework.

---

# Why This Technique Matters

Different teams frequently use the same words to mean different things.

Conversely, different words may be used to describe the same business concept.

For example:

```text
Customer
Client
Buyer
Account
Partner
```

may have very different meanings within one organisation.

Similarly:

```text
Revenue
Recognised Revenue
Booked Revenue
Billed Revenue
Forecast Revenue
Net Revenue
```

should not be assumed to mean the same thing.

Without agreed terminology, organisations can experience:

- Conflicting reports
- Inconsistent KPI calculations
- Data quality issues
- Misunderstood requirements
- Duplicate data models
- Poor search and discovery
- Difficult system integration
- Reduced trust in analytics
- Ambiguous AI responses

DAMA International maintains a standardised dictionary of data-management terminology specifically to promote consistency in the understanding and use of terms within the data-management profession (DAMA International, n.d.).

A Business Glossary applies the same principle to the language of an organisation.

---

# When to Use a Business Glossary

Business Glossary discovery is particularly useful when:

- Entering an unfamiliar business domain
- Multiple teams use different terminology
- Reports contain conflicting definitions
- KPIs are calculated differently
- New Data Products are being designed
- Systems are being integrated
- Data is being migrated
- An Enterprise Ontology is being created
- A semantic layer is being designed
- AI or conversational analytics capabilities are planned
- Business rules are poorly documented
- Ownership of information is unclear

Glossary development should begin early and continue throughout discovery.

It should not be treated as a one-off documentation exercise.

---

# What is a Business Term?

A Business Term represents a concept that has a specific meaning within the organisation.

Examples include:

```text
Customer
Programme
Contract
Campaign
Territory
Licence
Invoice
Revenue
Royalty
Forecast
Audience
Episode
```

A useful Business Term should have an agreed meaning that can be understood without needing to understand the underlying technical implementation.

---

# Business Glossary vs Data Dictionary

The terms Business Glossary and Data Dictionary are sometimes used interchangeably, but they serve different purposes.

| Business Glossary | Data Dictionary |
|-------------------|-----------------|
| Describes business meaning | Describes technical data structures |
| Business-facing | Primarily technical |
| Defines concepts and terminology | Defines fields, columns and data types |
| Independent of individual systems | Usually associated with a system or dataset |
| Supports shared understanding | Supports implementation and technical interpretation |

For example:

### Business Glossary

```text
Recognised Revenue

Revenue that has met the organisation's agreed criteria
for recognition within a defined accounting period.
```

### Data Dictionary

```text
Column: recognised_revenue_amount
Type: DECIMAL(18,2)
Nullable: No
Source: finance_revenue_fact
```

Both are valuable, but they answer different questions.

ISO/IEC 11179 defines metadata in terms of descriptions of data and provides a framework for registering and managing metadata items (ISO, 2023a; ISO, 2023b).

DISCOVER therefore treats the Business Glossary as the **business-semantic layer of understanding**, while technical metadata is captured separately within the Data Catalogue and related data documentation.

---

# Business Glossary vs Ontology

A glossary primarily answers:

> What does this term mean?

An ontology goes further and asks:

> How does this concept relate to other concepts?

For example:

```text
Glossary

Programme
    = A defined item of audiovisual content.
```

An ontology might additionally describe:

```text
Programme
    HAS Episode

Programme
    BELONGS TO Brand

Programme
    LICENSED THROUGH Contract

Programme
    DISTRIBUTED IN Territory

Programme
    GENERATES Revenue
```

The Business Glossary therefore provides important source material for ontology discovery.

---

# Shared Business Language

Domain-Driven Design emphasises the importance of developing a shared language between domain experts and technology teams and using that language consistently within the domain model (Evans, 2003).

DISCOVER applies this principle more broadly across business discovery.

Business terminology captured during workshops should therefore use language that:

- Business stakeholders recognise
- Product teams understand
- Analysts can apply
- Data teams can model
- Technology teams can implement
- AI systems can interpret

The objective is not simply to document terminology.

The objective is to establish a **shared business language**.

---

# What to Capture

For each Business Term consider capturing:

| Attribute | Purpose |
|-----------|---------|
| Term | Agreed business name |
| Definition | Meaning of the term |
| Description | Additional context |
| Domain | Business area in which it applies |
| Owner | Accountable business owner |
| Steward | Person responsible for maintaining it |
| Synonyms | Alternative terminology |
| Acronyms | Abbreviations |
| Related Terms | Associated business concepts |
| Business Rules | Rules that govern the concept |
| Examples | Practical examples |
| Status | Draft, Approved, Deprecated or Retired |

Additional metadata can be captured where it provides value.

---

# Writing Good Business Definitions

A good definition should be:

- Clear
- Concise
- Business focused
- Unambiguous
- Free from unnecessary technical terminology
- Understandable outside the immediate team

Avoid circular definitions.

Poor example:

```text
Customer

A person who is a customer of the organisation.
```

Better:

```text
Customer

An individual or organisation that purchases,
licenses or consumes a product or service provided
by the organisation.
```

The precise definition must reflect the organisation's own business model.

---

# Avoid System-Based Definitions

Business terms should describe the business rather than the current technology.

Avoid:

```text
Customer

A record stored in Salesforce.
```

Instead:

```text
Customer

An individual or organisation with which the
organisation has a defined commercial relationship.
```

Salesforce may be one system in which Customer information is represented, but the business concept exists independently of Salesforce.

This distinction becomes particularly important when systems are replaced or consolidated.

---

# Discovering Business Terms

Business terms can be identified from many sources.

Useful sources include:

- Stakeholder interviews
- Workshops
- Process maps
- Reports
- Dashboards
- KPI definitions
- Contracts
- Policies
- Data models
- Existing glossaries
- System interfaces
- Regulatory documentation
- Business capability maps

Listen carefully for terms that stakeholders:

- Repeat frequently
- Define differently
- Debate
- Qualify with additional words
- Use as acronyms
- Assume everybody understands

These often indicate important concepts.

---

# Generic Discovery Questions

## Understanding Terminology

- What are the most important terms used within this business area?
- Which terms would someone new to the organisation need to understand?
- Which terminology is unique to this business?
- Which acronyms are commonly used?
- Which terms are regularly misunderstood?

---

## Understanding Definitions

- What does this term mean?
- How would you explain it to someone outside your team?
- Is there an agreed definition?
- Where is the definition currently documented?
- Does everybody use this definition consistently?

---

## Identifying Conflicts

- Do other teams use this term differently?
- Are there multiple definitions?
- Which definition is considered authoritative?
- Does the meaning change depending on context?
- Has disagreement over this term caused reporting or operational problems?

---

## Understanding Ownership

- Who owns the definition?
- Who has authority to approve changes?
- Who should resolve disagreements?
- Who maintains the definition?
- Which governance forum should approve it?

---

## Understanding Relationships

- Which other business concepts relate to this term?
- Is this term part of a broader concept?
- Are there different types of this concept?
- What events affect it?
- Which processes create or consume it?

---

## Understanding Business Rules

- Are there rules associated with this concept?
- When does the concept become valid?
- Can its status change?
- Are there regulatory definitions that constrain it?
- Are exceptions allowed?

---

## Understanding Usage

- Which teams use this term?
- Which reports contain it?
- Which KPIs depend upon it?
- Which systems represent it?
- Which Data Products use it?

---

# Business Glossary Workshop

A glossary workshop may follow the structure below.

| Stage | Activity |
|-------|----------|
| 1 | Confirm business domain and scope |
| 2 | Identify important terms |
| 3 | Group related terminology |
| 4 | Discuss definitions |
| 5 | Identify synonyms and acronyms |
| 6 | Identify conflicting definitions |
| 7 | Identify ownership |
| 8 | Capture relevant business rules |
| 9 | Identify relationships |
| 10 | Agree items requiring further validation |

The objective is not necessarily to approve every definition during the workshop.

Terms can progress through a governance lifecycle.

For example:

```text
Proposed
    │
    ▼
Draft
    │
    ▼
Under Review
    │
    ▼
Approved
    │
    ▼
Deprecated
    │
    ▼
Retired
```

---

# Resolving Conflicting Definitions

Conflicting definitions are valuable discovery findings.

Do not immediately attempt to hide or merge them.

For example:

```text
Finance definition of Customer

vs

Sales definition of Customer

vs

Marketing definition of Customer
```

may reveal that each function is describing a legitimate but different business concept.

Further discovery might establish concepts such as:

```text
Prospect
Customer
Billing Customer
Licensee
Audience Member
Commercial Partner
```

The goal is semantic clarity rather than forcing all teams to use the same word regardless of context.

---

# Context Matters

Some terms legitimately have different meanings in different domains.

For example:

```text
Finance → Account
Sales   → Account
Digital → User Account
```

These should not automatically be merged.

Where meaning differs materially, the domain or context should be recorded.

Domain boundaries are therefore important when maintaining shared terminology.

---

# Glossary Governance

A useful Business Glossary requires governance.

Each important term should ideally have:

- An accountable owner
- A defined status
- A review process
- Version history
- Change control where appropriate

Governance should be proportionate.

Not every term requires executive approval.

Critical financial, regulatory or enterprise-wide definitions may require stronger controls than local operational terminology.

---

# Finance Example

## Discovery Objective

Establish a shared understanding of financial terminology used across reporting, planning, forecasting and revenue management.

Potential terms might include:

```text
Revenue
Recognised Revenue
Booked Revenue
Forecast Revenue
Actual Revenue
Accrued Revenue
Deferred Revenue
Gross Revenue
Net Revenue
Royalty
Margin
Cost
Budget
Forecast
Actual
```

### Example Questions

#### Revenue

- What does "Revenue" mean in this context?
- At what point is revenue recognised?
- Is recognised revenue different from booked revenue?
- What is the difference between gross and net revenue?
- How are cancellations treated?
- How are exchange rates applied?
- Which revenue definition is used in management reporting?
- Which definition is used for statutory reporting?

#### Forecasting

- What does "Forecast" mean?
- What is the difference between forecast and budget?
- How frequently is the forecast revised?
- What constitutes an actual?
- When does forecast information become actual information?

#### Ownership

- Who owns the official Revenue definition?
- Who owns the calculation rules?
- Can different Finance teams use different definitions?
- Who approves changes?

### Potential Findings

Discovery may reveal:

- Different reports use different revenue definitions.
- Sales and Finance use the term "Booked Revenue" differently.
- Manual adjustments are not reflected in documented definitions.
- Currency conversion rules vary by report.
- Ownership of KPI definitions is unclear.

### Potential Outputs

- Finance Business Glossary
- Revenue Definitions
- Finance KPI Catalogue
- Revenue Recognition Rules
- Ontology Concepts
- Semantic Layer Requirements

---

# Marketing Example

## Discovery Objective

Establish shared terminology for audiences, campaigns, channels, engagement and performance.

Potential terms might include:

```text
Campaign
Audience
Segment
Reach
Impression
Engagement
Conversion
Attribution
Channel
Lead
Customer
ROI
Acquisition
Retention
```

### Example Questions

#### Campaigns

- What constitutes a Campaign?
- Can one campaign span multiple channels?
- How is campaign start and end defined?
- Is a campaign the same concept across all marketing platforms?

#### Audiences

- What is an Audience?
- What is a Segment?
- How is a target audience different from an observed audience?
- Who owns audience definitions?

#### Performance

- What does Engagement mean?
- What constitutes a Conversion?
- How is Reach defined?
- How is campaign ROI calculated?
- Which attribution model is used?

### Potential Findings

Discovery may reveal:

- Platforms define engagement differently.
- Customer and audience terminology overlaps.
- Campaign identifiers are inconsistent across systems.
- Attribution terminology is poorly understood.
- Marketing and Finance calculate campaign return differently.

### Potential Outputs

- Marketing Business Glossary
- Audience Definitions
- Campaign Taxonomy
- Marketing KPI Catalogue
- Attribution Rules
- Marketing Ontology Concepts

---

# Connecting the Glossary to POPIT-V

The Business Glossary should be considered across all six POPIT-V perspectives.

### People

- Who owns definitions?
- Who creates terminology?
- Who consumes it?

### Organisation

- Which domains use the term?
- Is the definition enterprise-wide or domain-specific?

### Process

- Which processes create or change the concept?

### Information

- How is the concept defined and represented?

### Technology

- Which systems contain representations of the concept?

### Value

- Why is consistency important?
- What business problems arise from ambiguity?

---

# Connecting the Glossary to Other DISCOVER Artefacts

```text
Business Capability
        │
        ▼
Business Process
        │
        ▼
Business Terminology
        │
        ▼
Business Glossary
        │
        ├──────────────► KPI Catalogue
        │
        ├──────────────► Ontology
        │
        ├──────────────► Data Catalogue
        │
        ├──────────────► Semantic Layer
        │
        ├──────────────► Data Products
        │
        └──────────────► AI
```

The glossary therefore becomes an important semantic foundation for many later DISCOVER outputs.

---

# Supporting Ontology Discovery

Glossary discovery often begins to reveal relationships between concepts.

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

Programme
    DISTRIBUTED IN
Territory
```

These relationships should be captured and transferred into the Ontology Capture artefact.

The Business Glossary defines the concepts.

The Enterprise Ontology defines how those concepts relate.

---

# Supporting Data Products

Before designing a Data Product, confirm that important terminology is understood.

For example, a Revenue Data Product should not begin development while stakeholders disagree about:

```text
Revenue
Forecast
Actual
Territory
Customer
Contract
Currency
```

Resolving semantic ambiguity early reduces the risk of embedding conflicting definitions into analytical products.

---

# Supporting AI

AI systems that interact with organisational knowledge need context about business terminology.

A governed Business Glossary can therefore provide useful semantic context for:

- Enterprise Search
- Retrieval-Augmented Generation (RAG)
- Knowledge Assistants
- Conversational Analytics
- Metadata Generation
- Classification
- AI Agents

The glossary does not by itself guarantee correct AI behaviour, but it can provide a controlled source of organisational terminology and definitions.

---

# Common Pitfalls

## Creating a Technical Dictionary

Avoid turning the Business Glossary into a catalogue of database columns.

Technical metadata belongs primarily within the Data Catalogue or Data Dictionary.

---

## Copying Definitions Without Validation

Existing documentation can provide candidate definitions.

Do not assume those definitions are still correct.

Validate them with the business.

---

## Allowing Definitions Without Owners

Important definitions without ownership are difficult to govern.

---

## Trying to Define Everything

Not every word requires a glossary entry.

Prioritise terminology that is:

- Business critical
- Ambiguous
- Widely reused
- Required for reporting
- Required for integration
- Required for Data Products
- Required for AI

---

## Assuming One Definition Must Fit Every Domain

Some terminology is legitimately domain-specific.

Document context rather than forcing artificial standardisation.

---

## Writing Definitions Nobody Understands

A technically correct definition that business stakeholders cannot understand provides limited value.

Definitions should be written in business language.

---

# What Good Looks Like

A useful Business Glossary should:

- Be understandable by business users
- Contain agreed definitions
- Identify owners
- Capture important synonyms
- Identify conflicting terminology
- Record domain context
- Link related concepts
- Connect to KPIs and business rules
- Support ontology development
- Be governed and maintained
- Be easy to search and discover

---

# Discovery Outputs

Business Glossary discovery should contribute to:

- Business Glossary
- Term Catalogue
- Acronym Catalogue
- Definition Ownership
- Business Rules Catalogue
- KPI Catalogue
- Ontology Concepts
- Semantic Model Requirements
- Data Product Definitions
- Data Governance Requirements

---

# Related DISCOVER Artefacts

Business Glossary discovery should link to:

- Business Capability Map
- Stakeholder Register
- Process Maps
- Ontology Capture
- Data Catalogue
- KPI Catalogue
- RACI Matrix
- Data Product Canvas
- AI Opportunity Canvas
- Executive Summary

---

# Recommended Discovery Questions – Quick Reference

Before concluding glossary discovery, ensure you can answer:

- What are the critical business terms?
- What does each term mean?
- Does everybody interpret it consistently?
- Who owns the definition?
- Are synonyms used?
- Are different terms describing the same concept?
- Does the meaning vary by domain?
- Which business rules apply?
- Which KPIs depend upon it?
- Which processes use it?
- Which systems represent it?
- Which Data Products depend upon it?
- Should the term become part of the Enterprise Ontology?

---

# References

DAMA International (n.d.) *DAMA Dictionary of Data Management*. DAMA International. Available at: https://dama.org/learning-resources/dama-dictionary-of-data-management/ (Accessed: 10 August 2026).

DAMA International (n.d.) *Data Management Body of Knowledge (DAMA-DMBOK®)*. DAMA International. Available at: https://dama.org/learning-resources/dama-data-management-body-of-knowledge-dmbok/ (Accessed: 10 August 2026).

Evans, E. (2003) *Domain-Driven Design: Tackling Complexity in the Heart of Software*. Boston, MA: Addison-Wesley.

International Institute of Business Analysis (IIBA) (n.d.) *10.23 Glossary*. A Guide to the Business Analysis Body of Knowledge (BABOK® Guide). Available at: https://www.iiba.org/knowledgehub/business-analysis-body-of-knowledge-babok-guide/10-techniques/10-23-glossary/ (Accessed: 10 August 2026).

International Institute of Business Analysis (IIBA) (n.d.) *BABOK® Guide Appendix A: Glossary*. Available at: https://www.iiba.org/career-resources/a-business-analysis-professionals-foundation-for-success/babok/glossary/ (Accessed: 10 August 2026).

International Organization for Standardization (ISO) (2023a) *ISO/IEC 11179-1:2023 Information technology — Metadata registries (MDR) — Part 1: Framework*. Geneva: ISO.

International Organization for Standardization (ISO) (2023b) *ISO/IEC 11179-3:2023 Information technology — Metadata registries (MDR) — Part 3: Metamodel for registry common facilities*. Geneva: ISO.