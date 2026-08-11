---
title: "Business Glossary"
version: "1.2"
status: "Practitioner Technique"
---

# Business Glossary

> *"If two teams use the same word to mean different things, that disagreement is a discovery finding—not a documentation problem to hide."*

## Purpose

A Business Glossary creates a governed, business-readable catalogue of important terms and definitions.

Its purpose is to establish shared meaning where shared meaning is useful, and to make contextual differences visible where a single enterprise definition would be misleading.

## Why This Matters

Data initiatives often fail semantically before they fail technically.

Examples:

- “Customer” means buyer to Sales and billing party to Finance.
- “Revenue” means booked value, invoiced value and recognised value in different contexts.
- “Content” may refer to programme, episode, asset or format.
- “Available” may mean contractually available, operationally available or available after restrictions.

A glossary helps DISCOVER make these differences explicit.

## Glossary vs Data Dictionary vs Ontology

| Artefact | Primary concern |
|---|---|
| Business Glossary | Meaning of business terms |
| Data Dictionary | Technical data elements and structures |
| Taxonomy | Classification/hierarchy |
| Conceptual Model | Concepts and relationships |
| Ontology | Explicit semantics, relationships, constraints and concepts |
| Knowledge Graph | Connected instances/facts, often using an ontology |

A glossary is an excellent starting point for ontology discovery, but it is not itself an ontology.

## How It Fits DISCOVER

Useful in:

- Investigate;
- Study;
- Capture;
- Organise;
- Validate.

It becomes especially important when building:

- KPIs;
- cross-domain data products;
- semantic layers;
- ontologies;
- conversational analytics;
- AI agents.

## What to Capture for a Term

Recommended fields:

- Term ID;
- Preferred Term;
- Definition;
- Business Context;
- Synonyms;
- Acronyms;
- Example;
- Exclusions / non-examples;
- Related Terms;
- Owner;
- Steward / validator;
- Source / evidence;
- Status;
- Effective date;
- Notes;
- Linked ontology concept;
- Linked KPI/rule/data product where relevant.

## Writing Good Definitions

A useful definition should:

- use business language;
- distinguish the concept from related concepts;
- avoid circularity;
- avoid implementation detail;
- state important boundaries;
- be testable with examples.

Poor:

> Revenue is the revenue amount in the finance table.

Better:

> Revenue is economic value earned from an arrangement with a customer, measured according to the relevant accounting and commercial rules for the reporting context.

The exact definition must then be validated for the organisation.

## Discovery Process

### 1. Start from Decisions and Conversations

Capture terms that:

- matter to decisions;
- cause disagreement;
- appear in KPIs;
- cross teams;
- are used in contracts/rules;
- are important to data products.

### 2. Capture the Stakeholder Language

Do not normalise too early.

### 3. Draft Definitions

Use source material and subject-matter experts.

### 4. Identify Context

Ask whether the term has:

- one enterprise meaning;
- multiple legitimate contextual meanings;
- an informal and formal meaning.

### 5. Add Relationships

Link related terms and candidate ontology concepts.

### 6. Validate Ownership

Who can authoritatively approve the definition?

### 7. Govern Change

Definitions evolve. Capture status and effective dates where material.

## Generic Questions

- What does this term mean to you?
- Can you give a concrete example?
- What is explicitly not included?
- Does another team use the term differently?
- Is the definition formal or customary?
- Who owns it?
- Which report or rule depends on it?
- Which source provides the evidence?
- Has the definition changed over time?
- Does the definition vary by market, contract type or product?

## Conflicting Definitions

Do not resolve conflict by silently choosing one definition.

Record:

| Context | Definition | Owner | Evidence | Status |
|---|---|---|---|---|

Then determine whether:

- one definition is incorrect;
- both are legitimate in different bounded contexts;
- an enterprise concept with specialised sub-concepts is needed;
- a governance decision is required.

## Finance Example

Terms likely to require careful discovery:

- Revenue;
- Recognised Revenue;
- Billed Revenue;
- Forecast;
- Actual;
- Accrual;
- Adjustment;
- Contract;
- Licence;
- Period;
- FX Rate;
- Margin.

The glossary should link to relevant calculation and recognition rules rather than trying to encode every rule in the definition itself.

## Marketing Example

Potential terms:

- Campaign;
- Audience;
- Customer;
- Lead;
- Conversion;
- Reach;
- Frequency;
- Engagement;
- Attribution;
- Incrementality;
- Channel;
- Creative.

Different platforms may use similar metric names with materially different definitions.

## Glossary and AI

Conversational analytics and AI assistants need semantic grounding.

A governed glossary can help:

- improve retrieval;
- explain terms;
- map synonyms;
- prevent misleading KPI interpretation;
- route queries to the right context.

However, a glossary alone cannot guarantee correct AI answers. Provenance, access control, business rules and evaluation remain necessary.

## Outputs

- Business Glossary;
- Definition Conflict Log;
- Term Ownership Register;
- Synonym Map;
- Glossary-to-Ontology Mapping;
- Glossary governance process.

## Common Pitfalls

- copying database descriptions;
- defining everything in the enterprise;
- writing definitions in technical jargon;
- failing to record context;
- forcing one definition where several contexts are legitimate;
- no owner;
- no governance;
- creating the glossary once and never maintaining it;
- treating AI-generated definitions as authoritative.

## Practitioner Checklist

- [ ] Terms are business-significant.
- [ ] Definitions are understandable.
- [ ] Context is explicit.
- [ ] Synonyms are captured.
- [ ] Conflicts are preserved.
- [ ] Owner/validator is known.
- [ ] Evidence is referenced.
- [ ] Related concepts are linked.
- [ ] Change/governance is considered.
- [ ] Glossary supports decisions and data products rather than documentation volume.

## References

- DAMA International, *DAMA-DMBOK® 2nd Edition Revised*.
- International Institute of Business Analysis (IIBA), *BABOK® Guide, Version 3*.
- ISO/IEC 11179 series, *Metadata registries*.
- Business Architecture Guild (2026), *BIZBOK® Guide v15.0*.
- Evans, E. (2003), *Domain-Driven Design*. Addison-Wesley.

## Chapter Summary

The Business Glossary gives DISCOVER a shared language for the domain. Its real value is not the number of terms captured, but the semantic disagreements, ownership questions and reusable meaning it exposes.
