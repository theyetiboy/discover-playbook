# Selecting DISCOVER Artefacts

> **Purpose:** Preserve useful discovery knowledge without turning artefact completion into the objective.

---

# 1. Artefacts Exist to Preserve Learning

An artefact should help at least one of the following:

- create shared understanding;
- preserve evidence;
- expose disagreement;
- provide traceability;
- support validation;
- enable reuse;
- inform a decision;
- support governance.

If it does none of these, question why it exists.

---

# 2. Artefact Selection Question

Ask:

> **What knowledge will we create, and where is the most useful place to preserve it?**

Do not ask:

> "Which templates haven't we completed?"

---

# 3. Core Artefact Categories

## Engagement

- Discovery Brief
- Stakeholder Register
- Workshop Agenda
- RACI

## Business Model

- Capability Map
- Process Map
- Decision Catalogue
- Business Rules Catalogue
- Business Glossary
- Ontology Capture

## Evidence Control

- Evidence Register
- Assumption / Open Question Log
- Pain Point Register

## Data / Product

- Data Catalogue
- Data Product Canvas
- AI Opportunity Canvas

## Value / Prioritisation

- Opportunity Register
- Benefits / Value Register
- Maturity Assessment

## Traceability / Communication

- Golden Thread Traceability
- Executive Summary
- Executive Dashboard

---

# 4. Minimal Artefact Principle

Use the smallest useful set.

Example — first Finance orientation workshop:

Likely enough:

- Stakeholder Register;
- Capability Map;
- Evidence Register;
- Open Question Log.

Probably too early:

- Data Product Canvas;
- detailed Data Catalogue;
- AI Opportunity Canvas;
- Roadmap.

---

# 5. Artefact Selection by Discovery Objective

## Understand a Business Domain

Primary:

- Stakeholder Register;
- Capability Map;
- Evidence Register;
- Business Glossary;
- Decision Catalogue;
- Golden Thread.

Potential later:

- Process Maps;
- Business Rules;
- Maturity Assessment.

## Improve a Process

Primary:

- Process Map;
- Decision Catalogue;
- Pain Point Register;
- Evidence Register.

Supporting:

- Business Rules;
- Information requirements;
- Value Register.

## Design a Data Product

Primary:

- Data Product Canvas;
- Decision Catalogue;
- Information requirements;
- Data Catalogue;
- Benefits / Value Register;
- Golden Thread.

## Build an Ontology

Primary:

- Competency Questions;
- Business Glossary;
- Ontology Capture;
- Business Rules;
- Evidence Register.

## AI Opportunity

Primary:

- AI Opportunity Canvas;
- Process / task context;
- Decision Catalogue;
- Information requirements;
- Risk Register;
- Benefits / Value Register.

---

# 6. When to Create an Artefact

Create when:

- the knowledge will be reused;
- several stakeholders need the same view;
- the topic needs governance;
- the relationship is complex;
- traceability matters;
- validation will happen over time.

Avoid creating when:

- a simple note is sufficient;
- information is temporary;
- there is no owner or consumer;
- the artefact duplicates another source.

---

# 7. Stable IDs

Stable IDs are useful when artefacts need cross-reference.

Examples:

`CAP-001`  
`PRC-001`  
`DEC-001`  
`INF-001`  
`BR-001`  
`DAT-001`  
`VAL-001`

Supporting:

`EVD-001`  
`ASM-001`  
`OQ-001`  
`PAIN-001`  
`OPP-001`

Do not introduce IDs simply to make lightweight discovery look formal.

---

# 8. One Finding, Many Views

Avoid copying the same fact into five documents.

Capture the canonical record once, then reference it.

Example:

`DEC-014`

Decision Catalogue contains the authoritative decision record.

Process Map references `DEC-014`.

Golden Thread references `DEC-014`.

Data Product Canvas references `DEC-014`.

This is **Capture Knowledge Once, Reuse It**.

---

# 9. Evidence Should Travel With Findings

Where practical, every important artefact record should include:

- evidence;
- confidence;
- validation status;
- owner;
- related IDs.

This lets a reader distinguish:

- known;
- claimed;
- assumed;
- interpreted.

---

# 10. Artefact Lifecycle

Possible statuses:

- Unvalidated
- Validated
- Conflicted
- Superseded
- Closed

Do not delete disagreement merely because a preferred answer has emerged.

Preserve history where it matters.

---

# 11. Artefacts and NotebookLM

An AI assistant should:

- update the relevant artefact rather than create uncontrolled prose;
- preserve stable IDs;
- avoid duplicate records;
- mark unsupported values `UNKNOWN`;
- cite supplied evidence;
- preserve conflicting statements;
- identify artefacts that should change after new evidence.

The assistant should not invent business facts to complete a template.

---

# 12. Artefact Recommendation Format

When recommending an artefact, explain:

## Artefact

Decision Catalogue

## Why

The workshop needs to establish who makes the decision and what information/rules they use.

## Capture

- decision;
- owner;
- trigger;
- information;
- rules;
- action;
- evidence.

## Do Not Capture Yet

Detailed technical implementation.

---

# 13. Artefact Anti-Patterns

## Template Completion

"We completed 12 artefacts."

This says nothing about understanding.

## Duplicate Truth

Same KPI definition appears differently in three documents.

## Empty Governance

Artefacts have no owner or validator.

## Premature Product Artefact

A Data Product Canvas is completed before the consumer and decision are known.

## Decorative Traceability

IDs are added but do not connect meaningful business concepts.

---

# 14. Artefact Selection Checklist

- [ ] Artefact supports the objective.
- [ ] Consumer/owner exists.
- [ ] Knowledge is reusable.
- [ ] No existing canonical artefact already holds it.
- [ ] Evidence can be linked.
- [ ] Stable IDs used only where valuable.
- [ ] Validation status included.
- [ ] Artefact does not force premature solution design.
