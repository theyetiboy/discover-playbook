# DISCOVER Notebook Toolkit

This toolkit turns DISCOVER into an AI-assisted discovery capability for source-grounded assistants such as Google NotebookLM.

## Relationship to the Methodology

The files in `core/` are **derived operating material**.

The authoritative definition of DISCOVER lives in:

`docs/methodology/`

If the compact core or Notebook instructions conflict with the canonical methodology, the canonical methodology takes precedence.

---

## Recommended Notebook Pattern

### 1. DISCOVER Master Toolkit

Use this notebook for permanent methodology and reusable reference material.

Suggested sources:

- `00-DISCOVER-Core.md`
- `01-Notebook-Operating-Instructions.md`
- `02-Example-Prompt-Template.md`
- relevant domain prompt packs from `prompts/`
- selected canonical artefact templates from `docs/assets/templates/`
- worked examples where useful

The Master Toolkit is primarily for learning, preparation and reusable guidance.

### 2. Domain / Initiative Notebooks

Create a separate notebook for each meaningful discovery area, for example:

- Finance Discovery
- Rights Discovery
- Global Sales Discovery
- Content Discovery

Each domain notebook should contain:

- `00-DISCOVER-Core.md`
- `01-Notebook-Operating-Instructions.md`
- the relevant `Example-Prompt-<Domain>.md`
- only the canonical templates required for the engagement
- business documents
- process material
- data/reporting definitions
- workshop notes and transcripts
- decisions, assumptions and evidence collected during discovery

---

## Why Keep the Core Small?

The core should teach the notebook how DISCOVER works without overwhelming domain evidence.

Domain-specific sources provide the facts.

DISCOVER provides the method used to analyse them.

The notebook must not treat generic examples in the methodology or prompt packs as facts about the business domain currently being investigated.

---

## Recommended Canonical Templates

Load templates only when they are relevant.

Typical persistent discovery artefacts include:

- `decision_catalogue.md`
- `business_rules_catalogue.md`
- `evidence_register.md`
- `assumption_open_question_log.md`
- `pain_point_register.md`
- `opportunity_register.md`
- `benefits_value_register.md`
- `golden_thread_traceability.md`
- `data_product_canvas.md`
- `maturity_assessment.md`

Existing templates such as the Discovery Brief, Stakeholder Register, Capability Map, Business Glossary, KPI Catalogue and Data Catalogue can be added when needed.

---

## Traceability

For larger engagements, use stable IDs across artefacts.

Examples:

```text
CAP-003
PRC-012
DEC-008
INF-021
BR-004
DAT-015
DP-002
VAL-005
```

The notebook should preserve IDs once assigned.

If a new workshop changes the understanding of `DEC-008`, update the evidence, wording, confidence or validation state of `DEC-008`; do not automatically create another decision ID.

Supporting discovery records may use:

```text
EVD-
ASM-
OQ-
PAIN-
OPP-
RSK-
```

Use this only where the engagement benefits from persistent traceability.

---

## Suggested Operating Cycle

1. Load trusted sources.
2. Describe the discovery objective and stakeholders.
3. Ask the notebook to recommend the relevant DISCOVER stages and POPIT-V lenses.
4. Select only the artefact templates needed.
5. Generate a workshop or interview plan.
6. Conduct discovery.
7. Add notes, transcripts and supporting evidence.
8. Ask the notebook to structure findings using POPIT-V and the Golden Thread.
9. Update canonical artefacts while preserving stable IDs.
10. Validate findings with stakeholders.
11. Identify gaps, assumptions, contradictions and Broken Thread links.
12. Produce candidate opportunities only where evidence supports them.
13. Trace each recommendation backwards to business need and forwards to measurable Value.
14. Build an outcome-led roadmap when sufficient validated evidence exists.

---

## Important Principle

The notebook is a **discovery assistant**, not the source of business truth.

It should distinguish:

- evidence contained in supplied sources;
- statements made by stakeholders;
- assumptions;
- interpretations;
- recommendations;
- unresolved questions.

It should mark unknowns rather than filling gaps with general knowledge.

Where evidence conflicts, the conflict should remain visible until validated.
