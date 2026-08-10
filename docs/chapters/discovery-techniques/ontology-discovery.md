---
title: "Ontology Discovery"
version: "1.0"
author: "Steve Tarry"
technique: "Discovery Technique"
---

# Ontology Discovery

## Purpose

Ontology Discovery is the process of identifying the important business concepts within a domain, defining what those concepts mean and understanding the relationships and rules that connect them.

Within DISCOVER, ontology discovery is primarily a **business knowledge discovery technique**.

The objective is not to begin by designing a technical ontology.

The objective is to understand the business well enough that its knowledge can later be represented consistently in forms suitable for:

- Business Glossaries
- Semantic Layers
- Knowledge Graphs
- Data Products
- Analytics
- Artificial Intelligence
- Enterprise Search
- Data Integration

An ontology provides an explicit representation of a domain's concepts and the relationships between them. Gruber's influential definition describes an ontology as an explicit specification of a conceptualisation (Gruber, 1993).

Within DISCOVER, this idea is applied pragmatically:

> **What are the important things the business knows about, what do they mean, and how are they related?**

---

# Why This Technique Matters

Organisations contain large amounts of business knowledge.

That knowledge is often fragmented across:

- People
- Systems
- Reports
- Spreadsheets
- Policies
- Contracts
- Process documentation
- Data models
- Applications

Different business areas may also describe the same real-world concepts differently.

For example:

```text
Programme

Title

Content

Show

Production
```

may represent overlapping but distinct concepts.

Similarly:

```text
Customer

Client

Buyer

Licensee

Partner
```

may have different meanings depending upon the business context.

Ontology Discovery helps make these concepts and relationships explicit.

This can reduce semantic ambiguity and provide a stronger foundation for information modelling, Data Products and AI.

---

# When to Use Ontology Discovery

Ontology Discovery is particularly useful when:

- Business terminology is inconsistent
- Multiple systems represent similar concepts differently
- Data is fragmented across business domains
- An Enterprise Ontology is being developed
- A Knowledge Graph is planned
- A Semantic Layer is being designed
- New Data Products are being created
- Data integration is required
- Conversational analytics is planned
- AI Agents require business context
- Enterprise Search is being developed
- Business relationships are poorly understood
- Complex business rules need to be captured

Ontology Discovery becomes increasingly valuable as the number of business domains and data sources increases.

---

# What is an Ontology?

An ontology describes the concepts within a domain and the relationships that can exist between those concepts.

A simple example might be:

```text
Customer
    │
    └── SIGNS
            │
            ▼
         Contract
            │
            └── GRANTS
                    │
                    ▼
                  Rights
                    │
                    └── APPLY TO
                            │
                            ▼
                         Programme
```

The ontology does more than provide definitions.

It describes how concepts connect.

---

# Core Ontology Components

For DISCOVER purposes, an ontology can be understood through several simple building blocks.

## Concepts

Concepts represent important categories of things within the business.

Examples:

```text
Customer

Contract

Programme

Campaign

Invoice

Territory

Rights
```

In formal ontology languages such as OWL, categories are represented using **classes** (W3C, 2012).

---

# Instances

An Instance represents a specific example of a concept.

For example:

```text
Concept

Programme

Instance

Love Island
```

or:

```text
Concept

Territory

Instance

United Kingdom
```

Formal ontology languages commonly refer to these specific objects as **individuals** (W3C, 2012).

During early discovery, practitioners do not normally need to capture every instance.

Examples are primarily useful for validating whether the model makes sense.

---

# Relationships

Relationships describe how concepts are connected.

Examples:

```text
Customer
    SIGNS
Contract

Programme
    CONTAINS
Episode

Contract
    GRANTS
Rights

Programme
    DISTRIBUTED IN
Territory

Campaign
    PROMOTES
Programme
```

In OWL, relationships are represented through properties (W3C, 2012).

The relationship should have a clear business meaning.

Avoid vague relationships such as:

```text
RELATED TO
```

where a more precise relationship can be identified.

---

# Attributes

Attributes describe characteristics of a concept.

For example:

```text
Programme

Programme ID
Title
Genre
Duration
Status
```

or:

```text
Contract

Contract ID
Effective Date
Expiry Date
Currency
Status
```

During ontology discovery, attributes should only be captured where they help understand the business concept.

Detailed field-level modelling can be completed later.

---

# Business Rules

Business rules describe constraints or conditions that apply to concepts or relationships.

Examples:

```text
A Contract must have at least one Contract Party.

A Programme may contain multiple Episodes.

Rights may apply to one or more Territories.

Revenue may only be recognised when defined recognition criteria have been met.
```

Business rules add meaning beyond simple relationships.

---

# Hierarchies

Some concepts form hierarchical relationships.

For example:

```text
Content
│
├── Programme
│   ├── Series
│   └── Episode
│
└── Digital Content
    ├── Short Form Video
    └── Social Content
```

Hierarchies should represent meaningful business classification.

Do not create hierarchy simply because concepts appear related.

Knowledge-organisation standards such as SKOS distinguish hierarchical relationships such as broader and narrower concepts from associative relationships (W3C, 2009).

---

# Ontology vs Business Glossary

The Business Glossary answers:

> What does this concept mean?

Ontology Discovery additionally asks:

> How does this concept relate to everything else?

For example:

```text
BUSINESS GLOSSARY

Programme

A defined item of audiovisual content.
```

Ontology:

```text
Programme
    CONTAINS Episode

Programme
    BELONGS TO Brand

Programme
    LICENSED THROUGH Contract

Programme
    DISTRIBUTED IN Territory

Programme
    GENERATES Revenue
```

The glossary and ontology should therefore evolve together.

---

# Ontology vs Taxonomy

A Taxonomy primarily classifies concepts into hierarchical structures.

For example:

```text
Content
│
├── Scripted
│   ├── Drama
│   └── Comedy
│
└── Unscripted
    ├── Entertainment
    └── Factual
```

An ontology can represent hierarchy but also describes wider relationships.

For example:

```text
Programme
    HAS Genre

Programme
    PRODUCED BY Production Company

Programme
    LICENSED TO Customer

Programme
    AVAILABLE IN Territory
```

Ontology is therefore generally richer than taxonomy alone.

---

# Ontology vs Data Model

A Data Model describes how data is structured for a particular analytical, operational or technical purpose.

An ontology describes the underlying meaning of the business concepts and relationships.

For example:

```text
ONTOLOGY

Customer
    SIGNS
Contract
```

may be implemented across multiple physical data models:

```text
CRM

Account
Opportunity
Agreement

Finance

Customer_Master
Contract_Fact
Billing_Account
```

The ontology provides a business-semantic layer that is independent of a particular implementation.

---

# Ontology vs Knowledge Graph

An ontology defines the concepts, relationships and rules that describe a domain.

A Knowledge Graph applies those concepts and relationships to actual instances of data.

For example:

```text
ONTOLOGY

Programme
    DISTRIBUTED IN
Territory
```

A Knowledge Graph might contain:

```text
Love Island
    DISTRIBUTED IN
United Kingdom

Love Island
    DISTRIBUTED IN
Australia

Love Island
    DISTRIBUTED IN
United States
```

The ontology provides the model.

The Knowledge Graph contains knowledge expressed using that model.

---

# RDF Triple Thinking

A useful way of discovering relationships is to express them as simple three-part statements.

RDF represents information using **subject–predicate–object** triples (W3C, 2014).

DISCOVER can borrow this simple structure without requiring business participants to understand RDF.

For example:

```text
SUBJECT       RELATIONSHIP        OBJECT

Programme     HAS                 Episode

Contract      GRANTS              Rights

Rights        APPLY TO            Territory

Customer      SIGNS               Contract

Campaign      PROMOTES            Programme
```

This format is simple enough to use directly in business workshops.

---

# Start With Business Questions

Ontology Discovery should begin with the questions the organisation wants to answer.

Examples:

```text
Which customers have licensed this programme?

Which rights are available in Germany?

Which contracts generate revenue for this title?

Which territories can this format be sold into?

Which campaigns promoted this programme?

Which episodes belong to this series?
```

These questions expose the concepts and relationships needed within the model.

---

# Competency Questions

A useful ontology-development technique is to define questions that the ontology should eventually be capable of answering.

These are sometimes referred to as **competency questions** (Noy and McGuinness, 2001).

Examples:

```text
Which Programmes does Customer X license?

Which Contracts expire within the next 90 days?

Which Territories have available Rights for Programme Y?

Which Revenue is associated with a particular Contract?

Which Campaigns promoted Programme Z?
```

Competency questions help prevent ontology development from becoming an abstract modelling exercise.

If a concept or relationship does not help answer meaningful business questions, consider whether it belongs in the current scope.

---

# Discovering Concepts

Important concepts can be discovered from:

- Business Glossaries
- Stakeholder interviews
- Event Storming
- Process Maps
- Capability Maps
- Reports
- KPIs
- Data models
- Contracts
- Policies
- Source systems
- Domain-Driven Design workshops

Useful questions include:

- What are the important things this business works with?
- What nouns appear repeatedly?
- Which concepts have their own lifecycle?
- Which concepts need unique identities?
- Which concepts appear across several processes?
- Which concepts appear in multiple systems?

---

# Discovering Relationships

Once concepts have been identified, explore how they relate.

Ask:

- What does this concept belong to?
- What does it contain?
- What creates it?
- What does it create?
- Who owns it?
- What can it be associated with?
- What happens to it?
- What does it depend upon?

For example:

```text
Programme
```

might generate:

```text
Programme
    HAS Episode

Programme
    HAS Genre

Programme
    OWNED BY Brand

Programme
    PRODUCED BY Production Company

Programme
    LICENSED THROUGH Contract

Programme
    DISTRIBUTED IN Territory

Programme
    GENERATES Revenue
```

Each proposed relationship should be validated with Domain Experts.

---

# Relationship Direction

Relationships should be expressed clearly and directionally.

For example:

```text
Contract
    GRANTS
Rights
```

rather than:

```text
Contract
    RELATED TO
Rights
```

Where useful, consider the inverse relationship:

```text
Rights
    GRANTED BY
Contract
```

This can make the model easier to understand and query later.

---

# Discovering Rules

Ask stakeholders:

- Can this relationship always occur?
- Are there limits?
- Are there mandatory relationships?
- Can several of these exist?
- Are there exceptions?
- Does the rule vary by context?

For example:

```text
Programme
    HAS
Episode
```

may lead to:

```text
A Programme may contain zero or more Episodes.
```

while:

```text
Contract
    HAS
Contract Party
```

might require:

```text
Every Contract must have at least two Contract Parties.
```

The precise business rule must be validated rather than assumed.

---

# Discovering Lifecycle

Understanding lifecycle frequently exposes additional events and relationships.

For example:

```text
Contract

Draft
  │
  ▼
Negotiated
  │
  ▼
Approved
  │
  ▼
Signed
  │
  ▼
Active
  │
  ▼
Expired
```

Useful questions include:

- How is this concept created?
- Can it change?
- What statuses exist?
- What causes status changes?
- When is it retired?
- Can it be deleted?

Lifecycle information can connect ontology discovery with Event Storming and Process Modelling.

---

# Domain Boundaries

Ontology Discovery should not assume that one definition applies everywhere.

Domain-Driven Design shows why context matters.

For example:

```text
CUSTOMER

Sales Context
    Commercial Relationship

Finance Context
    Billing Entity

Marketing Context
    Audience / Consumer Relationship
```

Ontology Discovery should capture these distinctions where they are meaningful.

An Enterprise Ontology can then explicitly model how those concepts relate rather than hiding differences.

---

# Reuse Before Reinvention

Ontology development should consider whether relevant concepts already exist in:

- Existing enterprise models
- Industry standards
- Reference ontologies
- Internal glossaries
- Existing semantic models

Noy and McGuinness (2001) recommend considering reuse of existing ontologies as part of ontology development.

Reuse should not mean adopting an external model without validation.

The model must still accurately represent the organisation's business needs.

---

# Ontology Discovery Workshop

A DISCOVER Ontology Workshop might follow the structure below.

| Stage | Activity |
|-------|----------|
| 1 | Define domain and scope |
| 2 | Identify business questions |
| 3 | Identify important concepts |
| 4 | Agree initial definitions |
| 5 | Identify relationships |
| 6 | Identify hierarchies |
| 7 | Capture business rules |
| 8 | Explore lifecycle |
| 9 | Identify domain conflicts |
| 10 | Validate against competency questions |
| 11 | Identify ownership |
| 12 | Agree follow-up actions |

The workshop should remain conversational.

The facilitator should model what participants say rather than asking participants to learn ontology notation.

---

# Generic Discovery Questions

## Scope

- What business domain are we modelling?
- What problem are we trying to solve?
- Who will use this ontology?
- What questions should it help answer?
- What is explicitly out of scope?

---

## Concepts

- What are the most important business concepts?
- Which things have unique identity?
- Which concepts have their own lifecycle?
- Which concepts appear repeatedly?
- Which concepts are currently ambiguous?

---

## Definitions

- What does this concept mean?
- Does everyone agree?
- Does another domain define it differently?
- Who owns the definition?

---

## Relationships

- How does this concept relate to others?
- What does it contain?
- What belongs to it?
- What creates it?
- What does it create?
- What does it depend upon?

---

## Hierarchy

- Is this a type of another concept?
- Are there different categories?
- Is there a parent concept?
- Are there child concepts?

---

## Rules

- Which relationships are mandatory?
- Which are optional?
- Are there restrictions?
- What exceptions exist?
- Which rules are regulatory?

---

## Lifecycle

- How is the concept created?
- What causes it to change?
- Which statuses exist?
- When does it cease to exist?

---

## Ownership

- Who owns the concept?
- Who owns the definition?
- Who owns the underlying information?
- Who approves changes?

---

## Usage

- Which processes use this concept?
- Which capabilities depend upon it?
- Which systems represent it?
- Which KPIs use it?
- Which Data Products consume it?

---

# Finance Example

## Discovery Objective

Create a semantic model of the concepts and relationships required to understand commercial and financial performance.

An initial model might identify:

```text
Customer

Contract

Invoice

Revenue

Forecast

Actual

Currency

Territory

Royalty
```

Possible relationships:

```text
Customer
    SIGNS
Contract

Contract
    GENERATES
Invoice

Contract
    GENERATES
Revenue

Revenue
    REPORTED AS
Actual

Forecast
    PREDICTS
Revenue

Revenue
    DENOMINATED IN
Currency

Contract
    APPLIES TO
Territory

Revenue
    MAY GENERATE
Royalty
```

### Competency Questions

- Which contracts generate revenue for a customer?
- Which revenue is associated with a territory?
- What forecast exists for a contract?
- How does forecast compare with actual revenue?
- Which currencies are used?
- Which revenue generates royalty obligations?

### Example Questions

- What is the relationship between Contract and Revenue?
- Can one Contract generate multiple Revenue entries?
- Is Revenue associated directly with Customer or through Contract?
- How is Territory represented?
- How are currencies handled?
- What is the relationship between Forecast and Actual?
- How are royalties linked to revenue?
- Which rules determine revenue recognition?

### Potential Findings

Discovery may reveal:

- Revenue exists at several levels of granularity.
- Customer identity differs between Sales and Finance.
- Contracts can contain multiple rights and territories.
- Forecast information is modelled differently from actuals.
- Currency conversion introduces additional semantic rules.

### Potential Outputs

- Finance Ontology
- Revenue Ontology
- Finance Business Glossary
- Finance Semantic Model
- Finance Data Product Requirements
- Revenue Knowledge Graph Requirements

---

# Marketing Example

## Discovery Objective

Create a semantic model connecting campaigns, audiences, channels and outcomes.

Possible concepts:

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

Possible relationships:

```text
Campaign
    TARGETS
Audience

Audience
    CONTAINS
Segment

Campaign
    RUNS ON
Channel

Campaign
    USES
Creative

Campaign
    GENERATES
Impression

Impression
    MAY GENERATE
Engagement

Engagement
    MAY GENERATE
Conversion

Campaign
    INCURS
Spend

Conversion
    MAY GENERATE
Revenue
```

### Competency Questions

- Which campaigns target a particular audience?
- Which channels delivered a campaign?
- Which creatives generated the most engagement?
- Which campaigns generated conversions?
- Which campaigns generated the strongest return?

### Example Questions

- What constitutes a Campaign?
- Can one Campaign target multiple Audiences?
- How are Segments related to Audiences?
- Can one Creative appear in several Campaigns?
- What constitutes an Engagement?
- What constitutes a Conversion?
- How is Revenue attributed back to Campaign?
- Does terminology change by marketing platform?

### Potential Findings

Discovery may reveal:

- Channel platforms represent campaign concepts differently.
- Engagement has multiple definitions.
- Campaign IDs are not consistent across systems.
- Attribution relationships are complex.
- Audience and Customer models overlap but are not identical.

### Potential Outputs

- Marketing Ontology
- Campaign Semantic Model
- Audience Ontology
- Marketing Business Glossary
- Campaign Data Product Requirements

---

# Connecting Ontology Discovery to POPIT-V

Ontology Discovery is primarily associated with **Information**, but it connects to every POPIT-V perspective.

## People

- Who owns concepts?
- Who defines terminology?
- Who maintains business knowledge?

## Organisation

- Which domains use each concept?
- Where do semantic boundaries exist?

## Process

- Which processes create or modify concepts?
- Which events affect their lifecycle?

## Information

- What concepts, attributes, relationships and rules exist?

## Technology

- Which systems represent each concept?
- How are concepts mapped between systems?

## Value

- Which business questions can the ontology help answer?
- What decisions become easier?

---

# Connecting Ontology Discovery to Business Capability Mapping

Capabilities provide useful scope for ontology discovery.

For example:

```text
Rights Management
        │
        ▼
Important Concepts
        │
        ├── Rights
        ├── Contract
        ├── Territory
        ├── Programme
        └── Customer
```

This creates traceability between **what the organisation does** and **the information required to do it**.

---

# Connecting Ontology Discovery to Event Storming

Event Storming identifies important events.

Those events often expose concepts and relationships.

For example:

```text
Contract Signed
        │
        ▼
Rights Granted
        │
        ▼
Programme Licensed
```

may expose:

```text
Contract
    GRANTS
Rights

Rights
    APPLY TO
Programme
```

Event Storming therefore provides useful evidence for ontology discovery.

---

# Connecting Ontology Discovery to the Business Glossary

The Business Glossary and ontology should be developed together.

```text
Business Term
      │
      ▼
Definition
      │
      ▼
Ontology Concept
      │
      ▼
Relationships
```

The Glossary answers:

```text
What does Programme mean?
```

The ontology answers:

```text
How does Programme relate to Episode,
Contract, Rights, Territory and Revenue?
```

---

# Connecting Ontology Discovery to Data Products

A Data Product should use consistent business concepts.

For example:

```text
Rights Availability Data Product

Programme
Rights
Territory
Contract
Customer
```

If each of those concepts has an agreed semantic definition and relationship model, Data Product design becomes more consistent.

The ontology can therefore support:

- Product scope
- Semantic definitions
- Metric consistency
- Dataset integration
- API design
- Self-service analytics

---

# Connecting Ontology Discovery to AI

Ontology can provide structured context for AI systems.

Potential uses include:

- Enterprise Search
- Retrieval-Augmented Generation
- Knowledge Assistants
- Conversational Analytics
- AI Agents
- Metadata Generation
- Information Extraction

For example:

```text
User Question

"Where can we sell Programme X?"
```

Understanding this question may require relationships between:

```text
Programme
Rights
Territory
Contract
Availability
```

An ontology provides an explicit model of those relationships.

Formal knowledge representation can also support machine reasoning when the ontology contains sufficiently precise semantics.

However, ontology should not be presented as a guarantee of AI accuracy.

AI use cases still require independent evaluation, governance and testing.

---

# Moving Towards Formal Representation

Business discovery should remain implementation independent.

Once the business ontology is sufficiently mature, it may later be represented using standards such as:

- RDF
- RDFS
- OWL
- SKOS

RDF represents statements as subject–predicate–object triples (W3C, 2014).

OWL provides richer constructs for formally describing classes, properties, individuals and constraints (W3C, 2012).

SKOS provides a model particularly suited to controlled vocabularies, taxonomies and classification schemes (W3C, 2009).

The choice of formal representation should be driven by use cases rather than by the existence of a technology.

---

# Iterative Development

Ontology development is iterative.

Noy and McGuinness (2001) explicitly describe ontology development as an iterative process.

DISCOVER therefore expects the ontology to evolve:

```text
Discovery
    │
    ▼
Initial Concepts
    │
    ▼
Relationships
    │
    ▼
Validation
    │
    ▼
Additional Domains
    │
    ▼
Refinement
    │
    ▼
Governance
```

Do not attempt to create the complete Enterprise Ontology in one workshop.

Each discovery engagement should enrich the model.

---

# Governance

Important ontology concepts require governance.

Consider:

- Concept Owner
- Definition Owner
- Domain Owner
- Steward
- Change Approval
- Versioning
- Deprecation

Changes should be traceable, especially where concepts are reused by multiple Data Products or AI capabilities.

---

# Common Pitfalls

## Starting With Technology

Avoid starting with:

```text
Which graph database should we use?
```

Start with:

```text
What does the business need to understand?
```

Technology comes later.

---

## Modelling the Database

An ontology is not simply an Entity Relationship Diagram copied from an existing system.

Existing schemas can provide evidence, but the ontology should model business meaning.

---

## Trying to Model the Entire Enterprise

Start with a meaningful business scope.

Expand iteratively.

---

## Creating Concepts Without Business Questions

Use competency questions to keep modelling purposeful.

---

## Using Vague Relationships

Avoid excessive use of:

```text
RELATED TO
```

Prefer meaningful relationships such as:

```text
OWNS

CONTAINS

GRANTS

PRODUCES

USES

APPLIES TO
```

---

## Ignoring Domain Context

Do not force one definition across the enterprise where legitimate domain differences exist.

---

## Excessive Formalism During Discovery

Do not require business stakeholders to learn RDF, OWL or description logic.

Capture business knowledge first.

Formalisation can follow.

---

## No Ownership

An ontology with no business ownership will gradually lose trust.

---

# What Good Looks Like

Effective Ontology Discovery should produce:

- Clear scope
- Useful competency questions
- Identified business concepts
- Agreed definitions
- Meaningful relationships
- Relevant hierarchies
- Important business rules
- Lifecycle understanding
- Domain boundaries
- Identified ownership
- Traceability to business capabilities
- Traceability to Data Products
- Inputs into semantic modelling
- Inputs into AI knowledge design

The model should help stakeholders answer business questions more clearly than before discovery began.

---

# Discovery Outputs

Ontology Discovery should contribute to:

- Enterprise Ontology
- Domain Ontologies
- Business Glossary
- Concept Catalogue
- Relationship Catalogue
- Business Rules Catalogue
- Semantic Model
- Knowledge Graph Requirements
- Data Product Definitions
- Data Integration Requirements
- AI Knowledge Requirements

---

# Related DISCOVER Techniques

Ontology Discovery works particularly well alongside:

- Business Capability Mapping
- Business Glossary
- Domain-Driven Design
- Event Storming
- Process Modelling
- Stakeholder Mapping
- Data Product Design

A typical progression might be:

```text
Business Capability Mapping
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
    Ontology Discovery
            │
            ▼
     Semantic Model
            │
       ┌────┴────┐
       ▼         ▼
 Data Products   AI
```

The sequence is illustrative rather than mandatory.

---

# Recommended Discovery Questions – Quick Reference

Before concluding ontology discovery, ensure you can answer:

- What business questions should the ontology support?
- What domain is in scope?
- What are the important concepts?
- What does each concept mean?
- Who owns each concept?
- How are concepts related?
- Which hierarchies matter?
- Which business rules apply?
- What lifecycle does each concept have?
- Where do domain definitions differ?
- Which processes create or modify the concepts?
- Which capabilities depend upon them?
- Which systems represent them?
- Which KPIs use them?
- Which Data Products require them?
- Which AI use cases could benefit from them?
- What requires further validation?

---

# References

Gruber, T.R. (1993) 'A translation approach to portable ontology specifications', *Knowledge Acquisition*, 5(2), pp. 199–220.

Noy, N.F. and McGuinness, D.L. (2001) *Ontology Development 101: A Guide to Creating Your First Ontology*. Stanford, CA: Stanford Knowledge Systems Laboratory. Available at: https://protege.stanford.edu/publications/ontology_development/ontology101.pdf (Accessed: 10 August 2026).

World Wide Web Consortium (W3C) (2009) *SKOS Simple Knowledge Organization System Reference*. W3C Recommendation, 18 August. Available at: https://www.w3.org/TR/skos-reference/ (Accessed: 10 August 2026).

World Wide Web Consortium (W3C) (2012) *OWL 2 Web Ontology Language Primer (Second Edition)*. W3C Recommendation, 11 December. Available at: https://www.w3.org/TR/owl2-primer/ (Accessed: 10 August 2026).

World Wide Web Consortium (W3C) (2012) *OWL 2 Web Ontology Language Document Overview (Second Edition)*. W3C Recommendation, 11 December. Available at: https://www.w3.org/TR/owl2-overview/ (Accessed: 10 August 2026).

World Wide Web Consortium (W3C) (2014) *RDF 1.1 Concepts and Abstract Syntax*. W3C Recommendation, 25 February. Available at: https://www.w3.org/TR/rdf11-concepts/ (Accessed: 10 August 2026).