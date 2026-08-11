---
title: "Domain-Driven Design"
version: "1.2"
status: "Practitioner Technique"
---

# Domain-Driven Design

> *"A complex business domain becomes easier to understand when language, boundaries and models reflect the business rather than the database."*

## Purpose

Domain-Driven Design (DDD), introduced by Eric Evans, provides concepts for modelling complex business domains through close collaboration with domain experts.

DISCOVER uses selected DDD ideas primarily as **discovery and modelling tools**, not as a mandate to implement software using DDD patterns.

## Why This Matters

Large organisations frequently contain terms that change meaning by context.

For example:

- “Customer” in Sales may not equal “Customer” in Finance.
- “Content” in Production may not equal “Content” in Distribution.
- “Contract” in Legal may not equal the operational record used by Sales.

Trying to create one giant model too early can produce ambiguity.

DDD introduces useful concepts such as:

- Domain;
- Subdomain;
- Ubiquitous Language;
- Bounded Context;
- Context Map;
- Entity;
- Value Object;
- Aggregate;
- Domain Event.

## Strategic vs Tactical DDD

DISCOVER mainly benefits from **Strategic DDD**:

- identify domains/subdomains;
- understand language;
- identify bounded contexts;
- map relationships between contexts.

Tactical software patterns such as repositories or aggregates may become relevant later but should not dominate business discovery.

## Ubiquitous Language

A ubiquitous language is a shared language developed between domain experts and practitioners.

In DISCOVER this reinforces:

- Business Glossary;
- Ontology;
- EventStorming;
- conceptual modelling;
- source-to-business mapping.

The language should be grounded in how the business actually works.

## Bounded Context

A bounded context defines the boundary within which a model and language are consistent.

This is valuable when the same word has legitimate different meanings.

Example:

**Sales Context**
- Customer = commercial buyer.

**Finance Context**
- Customer = legal/billing party.

Rather than forcing one definition, model the relationship between the contexts.

## Subdomains

A domain can be divided into:

- **Core subdomain** — differentiating strategic capability;
- **Supporting subdomain** — necessary but not differentiating;
- **Generic subdomain** — common capability available externally.

Use these classifications carefully; they are strategic judgements requiring evidence.

## Context Mapping

A context map documents relationships between bounded contexts, including:

- information exchange;
- dependency;
- ownership;
- translation;
- shared concepts.

Within DISCOVER, the exact DDD relationship pattern names are less important than making the dependency and semantic translation explicit.

## How It Fits DISCOVER

Useful during:

- Investigate;
- Study;
- Capture;
- Organise;
- Validate;
- Evaluate.

Strong connections exist with:

- EventStorming;
- Ontology Discovery;
- Business Glossary;
- Capability Mapping;
- Data Product Design.

## Discovery Process

### 1. Define the Domain Question

What business area are we trying to understand?

### 2. Listen to Language

Capture terms and disagreements.

### 3. Identify Subdomains

Where do responsibilities, rules or language change?

### 4. Find Context Boundaries

Ask:

- Where is this definition valid?
- Who owns the model?
- Which team can change it?
- Where is translation required?

### 5. Map Context Relationships

Show information flowing between contexts.

### 6. Validate With Domain Experts

Boundaries are hypotheses until validated.

## Discovery Questions

- What is the core business domain?
- Which subdomains exist?
- Which parts are strategically differentiating?
- Where does terminology change?
- Where do rules change?
- Who owns the meaning?
- Which context is upstream for this information?
- Where is semantic translation required?
- Which context publishes information to others?
- Which concepts are genuinely shared?

## DDD and Data Products

DDD can help align data products to meaningful business domains.

Potential benefits:

- clearer ownership;
- coherent semantics;
- reduced cross-domain coupling;
- explicit data contracts;
- better product boundaries.

However:

> A bounded context is not automatically a data product, and a source system is not automatically a domain.

## DDD and Ontology

DDD and ontology solve related but different problems.

DDD emphasises model consistency **within boundaries**.

Ontology can make concepts and relationships **across boundaries** explicit.

DISCOVER can use both:

- DDD to preserve contextual meaning;
- ontology to connect concepts and support enterprise semantics.

## Finance Example

Potential contexts:

- Commercial / Sales;
- Contract / Rights;
- Financial Accounting;
- FP&A;
- Billing / Receivables.

“Revenue” may have different representations and lifecycle states across these contexts. Discovery should map translation and ownership rather than flattening them into one table definition.

## Marketing Example

Potential contexts:

- CRM / Customer;
- Media Buying;
- Campaign Planning;
- Web Analytics;
- Social;
- Brand.

The term “conversion” may differ by platform/context.

## Outputs

- Domain Map;
- Subdomain Catalogue;
- Bounded Context Map;
- Ubiquitous Language / Glossary;
- Context Relationship Map;
- Domain Events;
- Candidate Data Product Boundaries;
- Ontology mappings.

## Common Pitfalls

- applying software tactical patterns too early;
- treating organisational teams as permanent contexts without analysis;
- equating systems with bounded contexts;
- forcing one enterprise definition;
- creating boundaries without business evidence;
- using DDD jargon that stakeholders do not understand;
- designing microservices during discovery.

## Practitioner Checklist

- [ ] Domain question is clear.
- [ ] Language conflicts have been captured.
- [ ] Candidate contexts have business rationale.
- [ ] Ownership and rules are considered.
- [ ] Context relationships are explicit.
- [ ] System boundaries have not been assumed as domain boundaries.
- [ ] Data product implications remain hypotheses until validated.

## References

- Evans, E. (2003), *Domain-Driven Design: Tackling Complexity in the Heart of Software*. Addison-Wesley.
- Vernon, V. (2013), *Implementing Domain-Driven Design*. Addison-Wesley.
- Vernon, V. (2016), *Domain-Driven Design Distilled*. Addison-Wesley.
- Fowler, M., *Domain-Driven Design* (martinfowler.com).
- Brandolini, A., *Introducing EventStorming*.

## Chapter Summary

DDD gives DISCOVER a disciplined way to recognise business language, domain boundaries and semantic context. Used carefully, it prevents enterprise data design from flattening legitimate differences or mirroring current system boundaries.
