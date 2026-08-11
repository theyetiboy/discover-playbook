# DISCOVER™ Data Product Discovery Playbook

> A practical methodology for discovering business domains, creating shared understanding and translating evidence into valuable data, analytics and AI opportunities.

---

## Vision

DISCOVER is an open methodology for understanding business capabilities before designing technology.

It combines techniques from:

- Product Discovery
- Business Analysis
- Enterprise Architecture
- Domain-Driven Design
- Capability Mapping
- Process Modelling
- Data Product Thinking
- AI Opportunity Discovery

into a single repeatable framework.

DISCOVER is deliberately business-led, evidence-based, traceable and value-focused.

---

## Framework

DISCOVER consists of eight stages:

- **D**efine
- **I**nvestigate
- **S**tudy
- **C**apture
- **O**rganise
- **V**alidate
- **E**valuate
- **R**oadmap

The stages provide structure, but DISCOVER is iterative rather than a rigid waterfall. Learning can return the practitioner to an earlier stage whenever assumptions, definitions or relationships need to be revisited.

---

## Analytical Lens

DISCOVER uses **POPIT-V** to examine a business domain from six complementary perspectives:

- People
- Organisation
- Process
- Information
- Technology
- Value

Across an engagement, consider all relevant perspectives. Individual workshops should focus only on the perspectives required to achieve their objective.

---

## Golden Thread

DISCOVER preserves traceability from business intent to measurable value:

**Business Strategy**
→ **Business Capability**
→ **Business Process**
→ **Business Decision**
→ **Business Information**
→ **Business Rules**
→ **Technology / Data**
→ **Data Products / Analytics**
→ **Insight / Action**
→ **Business Value**

The Golden Thread is a traceability model, not a delivery lifecycle.

---

## Core Principles

**Business Before Technology**

**Start With Outcomes**

**Decisions Drive Data**

**Evidence Over Assumption**

**Validate Continuously**

**Value Always**

---

## Repository Architecture

The repository is deliberately organised into three representations of the methodology.

### Canonical Methodology — `docs/methodology/`

This is the authoritative definition of DISCOVER.

It contains the canonical descriptions of:

- the DISCOVER lifecycle;
- DISCOVER principles;
- POPIT-V;
- the Golden Thread;
- the maturity model.

If another file conflicts with the methodology, **`docs/methodology/` is the source of truth**.

See [`docs/methodology/README.md`](docs/methodology/README.md).

### Practitioner Playbook — `docs/chapters/` and `docs/assets/templates/`

These files explain how practitioners apply DISCOVER.

The chapters are human-readable guidance derived from the canonical methodology.

The template library provides reusable artefacts for workshops, evidence capture, traceability, opportunity evaluation and data product discovery.

### AI-Assisted Toolkit — `core/` and `prompts/`

These files are AI-optimised derivatives of the methodology for source-grounded assistants such as Google NotebookLM.

They define:

- how the AI should behave;
- how evidence should be classified;
- how workshops should be generated;
- how canonical artefacts should be updated;
- how domain prompt packs can be used.

The AI toolkit does **not** replace the canonical methodology and should not be treated as a source of business truth.

---

## Canonical Artefacts

DISCOVER uses only the artefacts needed to answer the discovery objective.

The template library includes, amongst others:

- Discovery Brief
- Stakeholder Register
- Business Capability Map
- Decision Catalogue
- Business Rules Catalogue
- Evidence Register
- Assumption & Open Question Log
- Pain Point Register
- Opportunity Register
- Benefits / Value Register
- Business Glossary
- KPI Catalogue
- Data Catalogue
- Golden Thread Traceability Matrix
- Data Product Canvas
- AI Opportunity Canvas
- Maturity Assessment
- Workshop Agenda

Artefacts should be linked where useful through the Golden Thread rather than maintained as isolated documents.

---

## Traceability

Larger engagements may use stable identifiers to connect artefacts, for example:

```text
STR-001  Strategic Objective
CAP-001  Business Capability
PRC-001  Business Process
DEC-001  Business Decision
INF-001  Information Requirement
BR-001   Business Rule
SYS-001  System / Technology
DAT-001  Data Asset
DP-001   Data Product
ACT-001  Business Action
VAL-001  Business Value
```

Supporting discovery records can use identifiers such as `EVD-`, `ASM-`, `OQ-`, `PAIN-` and `OPP-`.

Use this level of formality only where the size or complexity of the engagement justifies it.

---

## Notebook Toolkit

A recommended NotebookLM pattern is:

1. Load the compact DISCOVER core and operating instructions.
2. Add the relevant domain prompt pack.
3. Add only the canonical artefact templates needed for the engagement.
4. Add trusted business documents and workshop evidence.
5. Use the notebook to prepare discovery, structure findings and identify gaps.
6. Validate findings with stakeholders.
7. Preserve stable IDs when updating artefacts.
8. Trace recommendations to evidence and measurable value.

See [`core/README.md`](core/README.md).

A fictional end-to-end worked example is available at [`docs/examples/finance-simulation/`](docs/examples/finance-simulation/).

---

## Status

🚧 **Version 0.2 — Consolidation**

The methodology is actively evolving. The current focus is consistency between the canonical methodology, practitioner playbook, artefact library and AI-assisted toolkit.
