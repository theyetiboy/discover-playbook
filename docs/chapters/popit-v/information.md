---
title: "Information"
chapter: 14
version: "1.2"
status: "Practitioner Reference"
---

# Information

> *"Before modelling data, understand the meaning the business attaches to it."*

## Purpose

The **Information** perspective focuses on the information the business needs to operate and make decisions.

It includes business concepts, definitions, facts, documents, reports, KPIs, metadata, lineage, provenance, business rules and relationships.

The objective is not simply to identify databases or fields. It is to understand **meaning**: what the business is talking about, how information is interpreted, who owns that meaning and how trustworthy information supports decisions and outcomes.

## Why This Matters

Poor information management creates:

- multiple versions of the truth;
- conflicting KPI definitions;
- duplicate reporting;
- spreadsheet reconciliation;
- low trust;
- inconsistent decisions;
- duplicated data;
- manual interpretation;
- weak lineage;
- difficult integration;
- fragile AI and conversational analytics.

A technically correct data pipeline can still deliver the wrong business meaning.

Information discovery therefore precedes detailed physical data modelling.

## Discovery Objectives

Understand:

- critical business concepts;
- definitions and synonyms;
- conceptual relationships;
- information required by business decisions;
- KPIs and measures;
- business rules;
- documents and reports;
- authoritative sources;
- ownership and stewardship;
- quality expectations;
- timeliness/freshness;
- lineage and provenance;
- classifications and hierarchies;
- metadata;
- semantic conflicts;
- suitability for analytics and AI.

## What Good Looks Like

At the end of Information discovery you should be able to answer:

- What information is critical to the business area?
- Which decisions depend on it?
- What do the key business terms mean?
- Where do teams use different meanings?
- Who owns the definition?
- Which source is authoritative for which purpose?
- How is the information created and transformed?
- Which business rules affect it?
- How fresh and accurate must it be?
- How can users trace it back to evidence?
- Which reports and KPIs reuse the same concepts?
- Which concepts should become part of the shared ontology?

## What to Discover

### Business Concepts

Examples include:

- Customer;
- Contract;
- Right;
- Content;
- Licence;
- Territory;
- Revenue;
- Campaign;
- Opportunity;
- Forecast;
- Product.

Do not begin with table names. Start with the language used by the business.

### Definitions and Synonyms

Capture:

- preferred term;
- definition;
- synonyms;
- acronyms;
- context;
- examples;
- exclusions;
- owner;
- status;
- conflicting definitions.

A term may legitimately mean different things in different bounded contexts. DISCOVER should expose that rather than forcing false standardisation.

### Relationships

Explore:

- “is a” classifications;
- “part of” composition;
- ownership;
- participation;
- temporal relationships;
- contractual relationships;
- causal or dependency relationships;
- cardinality where useful;
- lifecycle states.

These relationships form the basis of a business concept model or ontology.

### Information Requirements

For each important decision ask:

- what facts are required;
- level of granularity;
- time horizon;
- freshness;
- history;
- comparison/benchmark;
- confidence or uncertainty;
- context;
- explanation;
- source.

### KPIs and Measures

Capture:

- business purpose;
- definition;
- formula;
- grain;
- time period;
- inclusion/exclusion rules;
- thresholds;
- targets;
- owner;
- source;
- consumers;
- decision/action supported.

A KPI without a decision or outcome is often just a metric.

### Business Rules

Rules can include:

- eligibility;
- classification;
- calculation;
- allocation;
- recognition;
- validation;
- approval;
- exception;
- compliance;
- prioritisation.

Separate the rule from the code, spreadsheet or SQL that currently implements it.

### Reports and Documents

Understand:

- purpose;
- consumers;
- decisions;
- cadence;
- manual effort;
- source;
- duplication;
- distribution;
- controls;
- retention;
- whether the report is still needed.

### Data Quality

Assess quality in relation to use.

Common dimensions include:

- accuracy;
- completeness;
- consistency;
- timeliness;
- validity;
- uniqueness;
- integrity.

Avoid declaring a dataset “high quality” without a use case and acceptable thresholds.

### Metadata, Lineage and Provenance

Capture:

- source;
- owner;
- transformation;
- calculation;
- timestamps;
- sensitivity;
- retention;
- lineage;
- evidence provenance;
- change history.

Provenance is particularly important where information is used for regulatory reporting, AI-generated answers or high-impact decisions.

### Authority and Trust

A “source of truth” statement is often too simplistic.

Ask:

- authoritative for which concept?
- for which time period?
- for which process?
- before or after adjustment?
- raw fact or approved reporting value?
- what happens when sources disagree?

## Generic Discovery Questions

### Business Information

- What information is essential for your team?
- What do you create?
- What do you receive?
- What do you share?
- Which information do you routinely challenge?

### Concepts

- What are the most important things in this domain?
- How do you define them?
- What distinguishes one from another?
- Which terms are overloaded?
- Which terms vary by market or business unit?
- What relationships matter?

### Decisions

- What information do you need to make this decision?
- At what level of detail?
- How current must it be?
- Do you need history, benchmark or forecast?
- What explanation is required?

### KPIs

- How do you measure success?
- How is the KPI calculated?
- What is included and excluded?
- Who owns the definition?
- Which targets or thresholds matter?
- Which KPI definitions are disputed?

### Rules

- Which rules change the meaning of the information?
- Where are the rules documented?
- Which rules are implemented in spreadsheets or code?
- Which rules vary by territory/customer/product?
- Who can approve a rule change?

### Quality

- Which information cannot be trusted?
- What does “wrong” mean in this use case?
- How often does the problem occur?
- Where is it detected?
- What business impact follows?
- What threshold would be acceptable?

### Lineage

- Where does the information originate?
- What transformations occur?
- Which manual adjustments are applied?
- Can a reported number be traced to evidence?
- Which lineage is currently unknown?


## Evidence to Capture

Do not treat workshop conversation as automatically validated fact. Capture important findings using the DISCOVER evidence model:

- **Evidence** — explicitly supported by a trusted source, observed artefact or validated record.
- **Stakeholder Statement** — stated by a stakeholder but not yet independently validated.
- **Assumption** — plausible but unverified.
- **Interpretation** — an analytical conclusion drawn from evidence.
- **Recommendation** — a proposed intervention.
- **Open Question** — information still required.

Where evidence conflicts, record the contradiction and identify who or what can validate it. Use `UNKNOWN` when an important Golden Thread link is not established.


## Glossary, Taxonomy, Concept Model and Ontology

These artefacts serve different purposes:

| Artefact | Primary purpose |
|---|---|
| Business Glossary | Shared definitions and terminology |
| Taxonomy | Controlled classification / hierarchy |
| Conceptual Model | Important concepts and relationships |
| Ontology | Explicit concepts, relationships, constraints and semantics |
| Logical Data Model | Structured representation for data design |
| Knowledge Graph | Instances/facts connected using a graph model, often informed by an ontology |

Do not call a list of tables an ontology.

## Discovery Artefacts

- Business Glossary;
- Information / Concept Catalogue;
- KPI Catalogue;
- Report Inventory;
- Business Rules Catalogue;
- Data Catalogue;
- Ontology Capture;
- Information Flow Diagram;
- Lineage / Provenance Map;
- Evidence Register;
- Golden Thread Traceability.

## Typical Pain Points

- conflicting definitions;
- unknown ownership;
- multiple sources of truth;
- spreadsheet calculations;
- duplicate reports;
- missing metadata;
- poor lineage;
- inconsistent identifiers;
- late data;
- manual adjustments;
- hidden rules;
- KPI disputes;
- semantic drift between teams;
- datasets optimised for systems rather than business use.

## Opportunities

- establish shared business terminology;
- define semantic ownership;
- standardise high-value measures;
- rationalise reporting;
- capture business rules;
- improve lineage and provenance;
- create reusable semantic models;
- build governed data products;
- create an enterprise/domain ontology;
- support trustworthy conversational analytics;
- improve metadata automation;
- introduce quality contracts aligned to decisions.

## Maturity Signals

### Fragmented
Definitions are tribal, spreadsheets dominate, lineage is unknown and reports disagree.

### Developing
Some catalogues and governance exist, but definitions and ownership vary.

### Defined
Important concepts, rules, KPIs, lineage and owners are documented and reusable.

### Managed
Quality and metadata are measured; semantic changes are governed; provenance is visible.

### Adaptive
Information is treated as a reusable enterprise asset; semantic models, data products and AI are continuously improved using governed feedback.

## Finance Example

### Discovery Focus

Understand the meaning and flow of financial information supporting forecasting, revenue recognition, actuals, planning and reporting.

### Concepts to Test

Do not assume these are universally defined:

- Contract;
- Licence;
- Revenue;
- Recognised Revenue;
- Billed Revenue;
- Forecast Revenue;
- Actual;
- Accrual;
- Adjustment;
- Cost;
- Margin;
- Territory;
- Period;
- Currency.

### Questions

- What event creates recognised revenue?
- How does treatment vary by contract type?
- Which date determines the accounting period?
- What is the authoritative contract information?
- Which adjustments occur after source-system data?
- How are FX rates selected?
- What is the relationship between sales value, invoiced value and recognised revenue?
- Which KPIs are externally versus internally reported?
- Can a reported number be traced back to a contract and rule?

### Outputs

- Finance Business Glossary;
- revenue concept model / ontology;
- Finance KPI Catalogue;
- Business Rules Catalogue;
- Finance data lineage;
- candidate governed data products.

## Marketing Example

### Discovery Focus

Understand campaign, customer/audience, channel, spend and performance concepts.

### Questions

- What is a campaign?
- What is the relationship between campaign, creative, placement, channel and audience?
- How are customer and audience segments defined?
- What constitutes a conversion?
- Which attribution rules are used?
- How are costs and outcomes joined?
- Which measures are comparable across channels?
- Which definitions differ between agency and internal reporting?


## Golden Thread Connection

This perspective should not exist as an isolated checklist. Connect findings to the Golden Thread wherever the evidence supports it:

**Business Strategy → Business Capability → Business Process → Business Decision → Business Information → Business Rules → Technology / Data → Data Product / Analytics → Insight / Action → Business Value**

Use stable identifiers when the engagement requires traceability:

- `STR-` Strategic Objective
- `CAP-` Business Capability
- `PRC-` Business Process
- `DEC-` Business Decision
- `INF-` Information
- `BR-` Business Rule
- `SYS-` System / Technology
- `DAT-` Data Asset
- `DP-` Data Product
- `ACT-` Business Action
- `VAL-` Business Value

Supporting discovery records may use `EVD-`, `ASM-`, `OQ-`, `PAIN-`, `OPP-` and `RSK-`.

The objective is traceability rather than bureaucracy. Do not invent links merely to complete the chain.


## Facilitation Cautions

- Start with business language, not data schemas.
- Preserve conflicting definitions until validated.
- Do not force enterprise-wide definitions where bounded-context differences are legitimate.
- Avoid “source of truth” shorthand without defining the context.
- Record rules separately from implementations.
- Treat AI-generated definitions as hypotheses unless validated.

## Practitioner Checklist

- [ ] Critical concepts are identified.
- [ ] Definitions and synonyms are captured.
- [ ] Owners/validators are known.
- [ ] Decisions are connected to information requirements.
- [ ] KPI formulas and rules are explicit.
- [ ] Authoritative sources are contextualised.
- [ ] Quality requirements are use-case specific.
- [ ] Lineage/provenance gaps are visible.
- [ ] Ontology relationships are evidence-based.
- [ ] AI/data product opportunities are downstream of semantic understanding.

## References

- DAMA International, *DAMA-DMBOK® 2nd Edition Revised* (2024 maintenance revision).
- ISO 8000 series, *Data quality*.
- ISO/IEC 11179 series, *Metadata registries (MDR)*.
- W3C, *RDF 1.2 Concepts and Abstract Data Model* (2026).
- W3C, *OWL 2 Web Ontology Language, Second Edition*.
- W3C, *PROV-O: The PROV Ontology*.
- W3C, *Data Catalog Vocabulary (DCAT) Version 3* (2024).
- Dehghani, Z. (2022), *Data Mesh*. O'Reilly.
- Evans, E. (2003), *Domain-Driven Design*. Addison-Wesley.

## Chapter Summary

The Information perspective ensures DISCOVER understands business meaning before technical representation. By linking concepts, definitions, rules, quality, lineage and ownership to decisions and outcomes, it creates the semantic foundation for trusted analytics, data products, ontology and AI.
