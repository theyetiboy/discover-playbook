---
title: "Ontology Discovery"
version: "1.2"
status: "Practitioner Technique"
---

# Ontology Discovery

> *"An ontology should model the business meaning that survives system change, not simply rename today's tables."*

## Purpose

Ontology Discovery identifies the important **business concepts, relationships, constraints, classifications and semantics** that describe a domain.

Within DISCOVER, ontology work starts as a business discovery activity. It may later be represented formally using semantic technologies, but the first objective is a shared and validated model of business meaning.

Ontology Discovery is particularly valuable where:

- many systems represent the same concepts differently;
- terminology changes by context;
- analytics must combine multiple domains;
- data products need reusable semantics;
- AI or conversational analytics must understand relationships;
- lineage needs to connect business meaning to physical data.

## Why This Matters

Traditional data integration often begins with schemas:

`customer_id`, `programme_code`, `contract_no`, `rev_amt`

but schemas do not explain:

- what a Customer is;
- whether a Programme is Content;
- how a Contract relates to a Licence;
- whether a Licence grants Rights;
- what Territory means;
- when Revenue becomes recognised;
- which concepts differ by business context.

An ontology creates an explicit layer of business meaning that can outlive the current platforms.

## What Is an Ontology?

At a practical business level, an ontology describes:

- **Concepts / Classes** — types of things in the domain;
- **Instances** — specific examples of those things;
- **Relationships / Properties** — how concepts are connected;
- **Attributes** — characteristics;
- **Hierarchies** — broader/narrower or class/subclass structures;
- **Constraints** — valid relationship patterns;
- **Business Rules** — logic that determines meaning or behaviour;
- **Terminology** — labels, synonyms and definitions.

Formal ontology languages such as OWL distinguish individuals, classes and properties. RDF provides a graph model for representing statements, while SKOS is useful for controlled vocabularies/taxonomies.

DISCOVER does not require formal OWL implementation. It requires semantic clarity.

## Concepts vs Instances

**Concept**
- Content
- Contract
- Territory
- Customer

**Instance**
- *Love Island* (specific content)
- Contract `C-10492`
- France
- Broadcaster X

Mixing instance data with the conceptual model can make workshops unnecessarily detailed.

## Ontology vs Other Artefacts

| Artefact | Primary Purpose | Example |
|---|---|---|
| Business Glossary | Define terms | "Licence" definition |
| Taxonomy | Classify | Genre hierarchy |
| Conceptual Model | Show major concepts/relationships | Contract relates to Party |
| Logical Data Model | Structure data for implementation | Entity/attribute design |
| Ontology | Explicit semantics, relationships and constraints | Licence grants Right in Territory |
| Knowledge Graph | Store/query connected facts/instances | Specific licence/territory/content facts |

The boundaries overlap, but the purpose differs.

## Ontology vs Taxonomy

A taxonomy primarily organises concepts into categories/hierarchies.

Example:

Content
- Scripted
  - Drama
  - Comedy
- Unscripted
  - Factual
  - Entertainment

An ontology can express richer relationships:

- Content **has Genre** Genre
- Party **owns** Right
- Licence **grants** Right
- Right **applies in** Territory
- Licence **has Window** TimePeriod

## Ontology vs Data Model

A physical/logical data model is often shaped by implementation concerns:

- keys;
- tables;
- normalisation;
- storage;
- performance.

An ontology focuses on domain meaning and relationships.

The ontology can inform data models, but should not simply mirror one.

## Ontology vs Knowledge Graph

An ontology can define the **schema/meaning**.

A knowledge graph typically contains **facts/instances** connected according to that meaning.

Example ontology:

`Licence --grants--> Right`

Example graph fact:

`Licence-123 --grants--> UK-Streaming-Right-456`

A knowledge graph can exist without a formal ontology, but governance and interoperability are usually stronger when semantics are explicit.

## Competency Questions

Competency questions are questions the ontology should be able to answer.

They are one of the most useful ways to keep ontology discovery business-led.

Examples:

- Which content is available for streaming in France next quarter?
- Which licences restrict exclusivity in Germany?
- Which customer has previously licensed this format?
- What revenue is associated with a given content title and territory?
- Which source and rule support this revenue value?
- Which rights expire before a proposed sales window?

A concept or relationship that supports no relevant business question may not need to be modelled yet.

## How Ontology Discovery Fits DISCOVER

### Define

Identify the business question and semantic scope.

### Investigate

Collect:

- existing terminology;
- glossaries;
- reports;
- contracts/policies;
- source schemas;
- domain models;
- stakeholder language.

### Study

Explore:

- concepts;
- relationships;
- rules;
- contexts;
- exceptions;
- identifiers.

### Capture

Record concepts and evidence using the Ontology Capture and Glossary templates.

### Organise

Build the conceptual/ontology model and connect it to Golden Thread IDs.

### Validate

Use domain experts to validate semantics.

### Evaluate

Assess gaps, conflicts, governance and reuse opportunities.

### Roadmap

Decide which semantic assets need implementation, governance or data mapping.

## POPIT-V Connections

### People
Who owns the meaning? Who validates concepts?

### Organisation
Which domain/capability owns each concept?

### Process
Where are concepts created or changed?

### Information
Definitions, relationships, rules and provenance.

### Technology
Which systems represent the concept and how?

### Value
Which decisions and outcomes become possible through shared semantics?

## Discovery Process

### Step 1 — Start With Business Questions

Write 5–20 competency questions.

Avoid starting with:

> "What tables do we have?"

Instead ask:

> "What does the business need to know or decide?"

### Step 2 — Identify Candidate Concepts

Mine:

- stakeholder language;
- capability maps;
- process models;
- reports;
- contracts/policies;
- KPIs;
- data catalogues.

### Step 3 — Define Concepts

For each concept capture:

- preferred name;
- definition;
- context;
- synonyms;
- owner;
- examples;
- exclusions;
- source/evidence.

### Step 4 — Identify Relationships

Ask:

- What can this be related to?
- What does it own?
- What is it part of?
- What grants/contains/produces it?
- What is the direction of the relationship?
- Is the relationship mandatory?
- Can there be many?

Do not add cardinality unless the business rule is sufficiently understood.

### Step 5 — Identify Classification and Hierarchy

Examples:

- Content type;
- Territory grouping;
- Customer type;
- Rights category.

Determine whether classifications are:

- authoritative;
- local;
- hierarchical;
- overlapping;
- time-dependent.

### Step 6 — Capture Rules and Constraints

Examples:

- a Licence may grant several Rights;
- a Right may be limited to one or more Territories;
- a Window has a start/end date;
- a Revenue Recognition Rule depends on contract terms.

Label unvalidated rules as hypotheses.

### Step 7 — Identify Context Boundaries

Ask where terms change meaning.

Use DDD bounded-context thinking where useful.

### Step 8 — Map to Source Data

Only after the business ontology is sufficiently clear.

Create mappings such as:

| Ontology Concept | Source System | Physical Object | Mapping Status |
|---|---|---|---|
| Content | System A | `title_master` | Candidate |
| Licence | System B | `agreement_line` | Needs validation |

Physical systems can change without redefining the business concept.

### Step 9 — Validate Against Competency Questions

Can the model explain the questions?

If not:

- missing concept?
- missing relationship?
- missing rule?
- missing provenance?
- wrong boundary?

### Step 10 — Establish Governance

Decide:

- owner;
- change process;
- versioning;
- approval;
- stewardship;
- publication;
- deprecation.

## Generic Ontology Discovery Questions

### Concepts

- What are the important things in this domain?
- Which concepts have business identity?
- How do you distinguish one from another?
- What examples can you provide?
- What is explicitly not this concept?

### Relationships

- How are these concepts connected?
- Can one exist without the other?
- Who/what owns or controls the relationship?
- Is the relationship time-dependent?
- Is it one-to-one, one-to-many or many-to-many?
- Are exceptions possible?

### Lifecycle

- What states can the concept be in?
- Which event changes the state?
- Can the state change backwards?
- Who is allowed to change it?

### Identity

- How does the business identify it?
- Do systems use different identifiers?
- Is there a trusted cross-reference?
- Can duplicates exist?

### Rules

- Which rules constrain relationships?
- Which rules depend on territory, customer or time?
- Where are they documented?
- Who owns them?

### Context

- Does the term mean the same thing everywhere?
- Which context owns the canonical meaning?
- Where is translation needed?

### Provenance

- Where did this fact come from?
- Which system/person/process created it?
- Which rule transformed it?
- Can the answer be traced back to evidence?

## Ontology Capture Example — Rights / Content

Candidate concepts:

- Content
- Programme
- Episode
- Format
- Party
- Contract
- Licence
- Right
- Territory
- Platform
- Window
- Restriction

Candidate relationships to validate:

- Programme **is a type of / represents** Content
- Episode **part of** Programme
- Contract **between** Parties
- Licence **created by / governed by** Contract
- Licence **grants** Right
- Right **relates to** Content
- Right **applies in** Territory
- Right **applies on** Platform
- Right **valid during** Window
- Right **subject to** Restriction

These are discovery hypotheses until validated by the organisation's business model.

## Finance Ontology Example

Potential concepts:

- Contract
- Licence
- Revenue
- Recognised Revenue
- Invoice
- Payment
- Forecast
- Actual
- Cost
- Currency
- Accounting Period
- Business Unit
- Territory

Competency questions:

- Which contract/licence facts explain this recognised revenue?
- Which recognition rule was applied?
- Which currency and rate were used?
- Which period contains the accounting event?
- Which adjustments changed the source value?

This creates business lineage beyond a table-level lineage tool.

## Marketing Ontology Example

Potential concepts:

- Campaign
- Audience
- Customer
- Segment
- Channel
- Creative
- Placement
- Impression
- Engagement
- Conversion
- Spend
- Outcome

Potential questions:

- Which audience was targeted by this campaign?
- Which creative ran on which channel?
- Which spend relates to the reported outcome?
- Which conversion definition applies?
- Which customer/segment relationship existed at the time?

## Ontology and the Golden Thread

Ontology primarily strengthens the Information portion of the Golden Thread, but it also connects across it.

Example:

`DEC-042 Should this content be pitched in France?`

requires:

`INF-101 Content`
`INF-102 Territory`
`INF-103 Right`
`INF-104 Window`
`INF-105 Customer`

with relationships defined by the ontology.

Those concepts map to:

`DAT-*` physical sources

and may support:

`DP-* Rights Availability Data Product`

leading to:

`ACT-* Create Sales Proposal`

and:

`VAL-* Increased Commercial Conversion / Reduced Search Time`.

## Ontology and Data Products

A data product should have clear semantic boundaries.

Ontology can help define:

- business concepts exposed;
- relationship semantics;
- ownership;
- identifiers;
- classification;
- contracts;
- interoperability with other products.

Do not build the ontology solely to support one dashboard if the concepts are enterprise-reusable.

## Ontology and AI / Agents

AI benefits from explicit semantics because users ask questions in business language.

Potential uses:

- semantic retrieval;
- entity linking;
- synonym resolution;
- relationship-aware search;
- grounding;
- explanation;
- query planning;
- metadata enrichment.

However an ontology does **not** remove the need for:

- access control;
- source provenance;
- data quality;
- evaluation;
- human oversight;
- current business rules.

## Formal Representation

DISCOVER remains implementation-neutral.

If formal semantic technology becomes valuable, common standards include:

### RDF
A graph data model for representing statements.

### RDFS
Basic schema/class/property semantics.

### OWL 2
A formal ontology language supporting classes, properties, individuals and richer semantics.

### SKOS
Useful for controlled vocabularies and concept schemes.

### SHACL
Useful for describing/validating RDF graph constraints.

### PROV-O
Useful for modelling provenance.

### DCAT
Useful for data catalogue semantics.

The implementation level should be proportionate to the use case.

## Ontology Governance

Define:

- domain owner;
- semantic steward;
- approval process;
- change request;
- version;
- effective date;
- deprecated concepts;
- mapping ownership;
- quality checks.

A semantic model without governance will drift.

## Common Pitfalls

### Starting From Tables

This reproduces physical design instead of business meaning.

### Modelling Everything

Ontology scope should be driven by competency questions and value.

### Premature Formalism

Do not debate OWL profiles while stakeholders still disagree what a Licence means.

### False Enterprise Standardisation

Different bounded contexts may legitimately require different definitions.

### Invented Relationships

AI and analysts can easily propose plausible relationships. They remain assumptions until validated.

### No Provenance

A relationship without source/owner becomes difficult to trust.

### No Change Process

Business semantics evolve.

## Outputs

- Competency Question Catalogue;
- Business Glossary;
- Concept Catalogue;
- Ontology Capture;
- Concept Relationship Model;
- Context Map;
- Classification / Taxonomy;
- Business Rules Catalogue;
- Source-to-Concept Mapping;
- Semantic Governance Model;
- Golden Thread Traceability.

## What Good Looks Like

A good ontology:

- answers relevant business questions;
- uses business language;
- distinguishes concepts from instances;
- makes relationships explicit;
- preserves context;
- has ownership;
- links to evidence;
- maps to physical data without depending on it;
- evolves through governance;
- is usable by humans before machines.

## Practitioner Checklist

- [ ] Competency questions exist.
- [ ] Concepts are business-defined.
- [ ] Instances are not confused with classes.
- [ ] Relationships are explicit and directional.
- [ ] Cardinality/constraints are evidence-based.
- [ ] Context differences are preserved.
- [ ] Owners and evidence are recorded.
- [ ] Source-system mappings are separate from definitions.
- [ ] Provenance requirements are understood.
- [ ] Governance/versioning is defined.
- [ ] AI/data product uses are traceable to value.

## References

- Noy, N.F. & McGuinness, D.L. (2001), *Ontology Development 101: A Guide to Creating Your First Ontology*. Stanford University.
- W3C, *OWL 2 Web Ontology Language Primer, Second Edition*.
- W3C, *RDF 1.2 Concepts and Abstract Data Model* (2026).
- W3C, *SKOS Simple Knowledge Organization System Reference*.
- W3C, *PROV-O: The PROV Ontology*.
- W3C, *Data Catalog Vocabulary (DCAT) Version 3*.
- Evans, E. (2003), *Domain-Driven Design*. Addison-Wesley.
- Grüninger, M. & Fox, M.S. (1995), methodology work on ontology design and competency questions.
- DAMA International, *DAMA-DMBOK® 2nd Edition Revised*.

## Chapter Summary

Ontology Discovery turns fragmented business terminology into an explicit, connected semantic model. By starting with competency questions and business meaning, DISCOVER can build a semantic layer that supports integration, governed data products, lineage, analytics and AI without simply reproducing today's systems.
