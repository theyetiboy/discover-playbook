# DISCOVER™ Data Product Discovery Playbook

> A practical methodology for understanding business domains, creating shared understanding and translating evidence into valuable data, analytics and AI outcomes.

DISCOVER is designed for practitioners working at the intersection of business analysis, product management, data, analytics, architecture and AI.

It is deliberately:

- **business-led** — understand the outcome and capability before choosing technology;
- **decision-led** — decisions drive information and data requirements;
- **evidence-based** — distinguish what is known from what is assumed;
- **semantic** — model business meaning, not only systems and schemas;
- **traceable** — connect discovery through the Golden Thread;
- **iterative** — validate continuously rather than operate as a waterfall;
- **value-focused** — every recommendation must ultimately answer **“So what?”**

---

# DISCOVER Lifecycle

**DISCOVER** =

1. **D — Define**
2. **I — Investigate**
3. **S — Study**
4. **C — Capture**
5. **O — Organise**
6. **V — Validate**
7. **E — Evaluate**
8. **R — Roadmap**

The lifecycle provides structure without becoming a stage-gate process.

> Do not progress on the basis of critical untested assumptions. Establish sufficient confidence to move forward, validate continuously and return to earlier stages whenever learning requires it.

---

# POPIT-V Analytical Lens

DISCOVER examines the business through six complementary perspectives:

- **People**
- **Organisation**
- **Process**
- **Information**
- **Technology**
- **Value**

Across an engagement, consider all relevant perspectives.

An individual interview or workshop **does not need to explore all six**. Select only the perspectives necessary to achieve the session objective.

---

# The Golden Thread

DISCOVER connects business intent to measurable value:

```text
Business Strategy
        ↓
Business Capability
        ↓
Business Process
        ↓
Business Decision
        ↓
Business Information
        ↓
Business Rules
        ↓
Technology / Data
        ↓
Data Products / Analytics
        ↓
Insight / Action
        ↓
Business Value
```

The Golden Thread is a **traceability model**, not a delivery lifecycle.

A missing or unsupported relationship is a **Broken Thread**. DISCOVER makes Broken Threads visible rather than filling them with assumptions.

---

# Core Principles

1. **Business Before Technology**
2. **Start With Outcomes**
3. **Decisions Drive Data**
4. **Model the Business, Not the Systems**
5. **Understand People in Context**
6. **Evidence Over Assumption**
7. **Create Shared Understanding**
8. **Capture Knowledge Once, Reuse It**
9. **Connect Everything**
10. **Explore Before You Converge**
11. **Remain Solution Neutral**
12. **Validate Continuously**
13. **Design Governance In**
14. **Every Recommendation Must Deliver Value**

See [`docs/methodology/discover-principles.md`](docs/methodology/discover-principles.md).

---

# Evidence Model

Important findings should be distinguishable as:

- **Evidence**
- **Stakeholder Statement**
- **Assumption**
- **Interpretation**
- **Recommendation**
- **Open Question**

Where a material fact is unknown, DISCOVER explicitly permits:

```text
UNKNOWN
```

Where evidence conflicts, preserve the conflict and create a validation question.

---

# Repository Architecture

The repository has three complementary representations of the methodology.

## 1. Canonical Methodology — `docs/methodology/`

This is the authoritative definition of DISCOVER.

It contains:

- the full DISCOVER framework;
- DISCOVER principles;
- POPIT-V;
- the Golden Thread;
- maturity model;
- change-control guidance.

**If another file conflicts with `docs/methodology/`, the methodology directory is authoritative.**

Start with:

[`docs/methodology/README.md`](docs/methodology/README.md)

## 2. Practitioner Playbook — `docs/`

Human-readable practitioner material:

```text
docs/
├── methodology/        # canonical methodology
├── chapters/           # practitioner chapters
│   ├── popit-v/
│   ├── discovery-techniques/
│   └── references/
├── assets/templates/   # reusable canonical artefacts
├── examples/           # worked examples
└── appendices/         # questions, agendas, checklists, glossary, reading
```

Start with:

[`docs/README.md`](docs/README.md)

## 3. AI-Assisted Toolkit — `core/` and `prompts/`

AI-optimised material for source-grounded assistants such as Google NotebookLM.

```text
core/
├── 00-DISCOVER-Core.md
├── 01-Notebook-Operating-Instructions.md
└── 02-Example-Prompt-Template.md

prompts/
├── Example-Prompt-Finance.md
├── Example-Prompt-Rights.md
├── Example-Prompt-Global-Sales.md
├── Example-Prompt-Content.md
└── Example-Prompt-Marketing.md
```

The AI toolkit helps prepare workshops, structure evidence and maintain artefacts.

It is **not the source of business truth**.

---

# Practitioner Chapters

The main playbook covers:

1. Introduction
2. DISCOVER Lifecycle
3. Engagement Preparation
4. POPIT-V Overview
5. Workshop Playbook
6. Discovery Techniques
7. Data Product Design
8. AI Opportunity Discovery
9. Prioritisation
10. Roadmapping

The enriched POPIT-V field guides cover:

- People
- Organisation
- Process
- Information
- Technology
- Value

The discovery technique library covers:

- Business Capability Mapping
- Stakeholder Mapping
- Process Modelling
- Value Stream Mapping
- EventStorming
- Business Glossary
- Domain-Driven Design
- Wardley Mapping
- Ontology Discovery

---

# Canonical Artefact Library

Use the **smallest set of artefacts that answers the discovery objective**.

The template library includes:

### Engagement & Facilitation

- Discovery Brief
- Stakeholder Register
- Workshop Agenda
- RACI / Responsibility Matrix

### Business Understanding

- Capability Map
- Decision Catalogue
- Business Rules Catalogue
- Business Glossary
- KPI Catalogue
- Ontology Capture

### Evidence & Discovery Control

- Evidence Register
- Assumption / Open Question Log
- Pain Point Register

### Information, Technology & Product

- Data Catalogue
- Data Product Canvas
- AI Opportunity Canvas

### Opportunity & Value

- Opportunity Register
- Benefits / Value Register
- Maturity Assessment

### Traceability & Communication

- Golden Thread Traceability
- Executive Summary
- Executive Discovery Dashboard

See:

[`docs/assets/templates/README.md`](docs/assets/templates/README.md)

---

# Traceability IDs

For persistent or complex discovery, stable identifiers may be used.

| Prefix | Meaning |
|---|---|
| `STR-` | Strategic Objective |
| `CAP-` | Business Capability |
| `PRC-` | Business Process |
| `DEC-` | Business Decision |
| `INF-` | Business Information |
| `BR-` | Business Rule |
| `SYS-` | System / Technology |
| `DAT-` | Data Asset |
| `DP-` | Data Product |
| `ACT-` | Business Action |
| `VAL-` | Business Value |

Supporting records:

| Prefix | Meaning |
|---|---|
| `EVD-` | Evidence |
| `ASM-` | Assumption |
| `OQ-` | Open Question |
| `PAIN-` | Pain Point |
| `OPP-` | Opportunity |
| `RSK-` | Risk |

Do not force IDs into lightweight discovery where they create more administration than value.

---

# Maturity Model

DISCOVER assesses maturity **separately across each POPIT-V dimension**:

1. **Fragmented**
2. **Developing**
3. **Defined**
4. **Managed**
5. **Adaptive**

Prefer a maturity profile rather than a single averaged score.

See:

[`docs/methodology/maturity-model.md`](docs/methodology/maturity-model.md)

---

# NotebookLM / Source-Grounded AI Pattern

A practical pattern:

## Master Toolkit Notebook

Load:

1. `core/00-DISCOVER-Core.md`
2. `core/01-Notebook-Operating-Instructions.md`
3. relevant templates
4. relevant domain prompt packs
5. selected methodology/practitioner sources

Use it to understand and apply DISCOVER.

## Domain / Initiative Notebook

For a Finance, Rights, Global Sales, Content or other discovery:

1. load the compact DISCOVER core/instructions;
2. load the relevant prompt pack and templates;
3. add trusted business documents;
4. add workshop/interview evidence;
5. ask the notebook to structure findings;
6. validate with stakeholders;
7. maintain stable IDs and Broken Threads.

The notebook must distinguish **source evidence from inference**.

See:

[`core/README.md`](core/README.md)  
[`prompts/README.md`](prompts/README.md)

---

# Worked Example

The fictional Finance simulation demonstrates:

```text
Discovery Brief
      ↓
Workshop Plan
      ↓
Mock Workshop Notes
      ↓
POPIT-V / Artefact Analysis
      ↓
Golden Thread
      ↓
Outcome-Led Roadmap
```

It deliberately begins with unvalidated assumptions such as:

- “We need a dashboard.”
- “AI might improve forecasting.”
- “Poor data quality is probably the problem.”

DISCOVER tests rather than accepts those statements.

See:

[`docs/examples/finance-simulation/README.md`](docs/examples/finance-simulation/README.md)

---

# References

DISCOVER is informed by established work including:

- IIBA BABOK® Guide;
- Business Architecture Guild BIZBOK® Guide;
- DAMA-DMBOK®;
- TOGAF®;
- BPMN / DMN;
- Domain-Driven Design;
- EventStorming;
- Lean / Value Stream Mapping;
- W3C semantic-web standards;
- ISO AI / information-security standards;
- NIST AI Risk Management Framework;
- product discovery and strategy literature.

The repository distinguishes external method/reference material from organisation-specific discovery evidence.

See:

[`docs/chapters/references/`](docs/chapters/references/)  
[`docs/appendices/appendix_F_reading_list.md`](docs/appendices/appendix_F_reading_list.md)

---

# Baseline Status

**Baseline Candidate v1.0 — 11 August 2026**

This candidate consolidates:

- the enriched DISCOVER methodology and practitioner playbook;
- POPIT-V field guides;
- enriched discovery-technique chapters;
- canonical artefact templates;
- evidence and traceability model;
- Golden Thread / Broken Threads;
- outcome-led roadmapping;
- data product and AI discovery;
- NotebookLM operating instructions and prompt packs;
- Finance worked simulation;
- refreshed reference library.

See [`BASELINE.md`](BASELINE.md).

---

# Licensing

See [`LICENSE.md`](LICENSE.md).

Names and trademarks belonging to third parties remain the property of their respective owners.
