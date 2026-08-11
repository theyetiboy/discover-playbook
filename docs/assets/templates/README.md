# DISCOVER Canonical Artefact Templates

This directory contains reusable artefacts for applying DISCOVER.

## Principle

**Use the smallest set of artefacts that answers the discovery objective.**

The template library is not a checklist.

A practitioner should not create every artefact simply because a template exists.

## Canonical Template Behaviour

Where a template is used:

- preserve the structure unless the engagement has a justified need to extend it;
- preserve existing IDs when updating records;
- mark unsupported information as `UNKNOWN`;
- link records to evidence where possible;
- distinguish stakeholder statements from validated evidence;
- make conflicts visible;
- record confidence and validation status where relevant;
- connect artefacts through the Golden Thread rather than maintaining isolated documents.

## Core Traceability IDs

For larger engagements:

| Prefix | Artefact |
|---|---|
| `STR-` | Strategic Objective |
| `CAP-` | Business Capability |
| `PRC-` | Business Process |
| `DEC-` | Business Decision |
| `INF-` | Information Requirement / Concept |
| `BR-` | Business Rule |
| `SYS-` | System / Technology |
| `DAT-` | Data Asset |
| `DP-` | Data Product |
| `ACT-` | Business Action |
| `VAL-` | Business Value |

Supporting discovery records:

| Prefix | Artefact |
|---|---|
| `EVD-` | Evidence Item |
| `ASM-` | Assumption |
| `OQ-` | Open Question |
| `PAIN-` | Pain Point |
| `OPP-` | Opportunity |
| `RSK-` | Risk |

Use a zero-padded sequence such as `DEC-001`.

IDs should be stable. A change in wording or validation status does not automatically create a new ID.

## Evidence / Validation Status

Recommended values where a status field is useful:

- `Unvalidated`
- `Validated`
- `Conflicted`
- `Superseded`
- `Closed`

Recommended confidence values:

- `Low`
- `Medium`
- `High`

Confidence should reflect the strength of evidence, not how strongly a stakeholder expressed an opinion.

## Template Index

### Engagement and Facilitation

- `discovery_brief.md`
- `stakeholder_register.md`
- `workshop_agenda.md`
- `RACI.md`

### Business Understanding

- `capability_map.md`
- `decision_catalogue.md`
- `business_rules_catalogue.md`
- `business_glossary.md`
- `kpi_catalogue.md`
- `ontology_capture.md`

### Evidence and Discovery Control

- `evidence_register.md`
- `assumption_open_question_log.md`
- `pain_point_register.md`

### Information and Technology

- `data_catalogue.md`

### Opportunity, Value and Product

- `opportunity_register.md`
- `benefits_value_register.md`
- `data_product_canvas.md`
- `ai_opportunity_canvas.md`
- `maturity_assessment.md`

### Traceability and Communication

- `golden_thread_traceability.md`
- `executive_summary.md`
- `executive_dashboard.md`

## AI-Assisted Use

When these templates are loaded into a source-grounded notebook, instruct the AI to:

1. use the supplied canonical structure;
2. reuse existing IDs;
3. create new IDs only for genuinely new records;
4. cite or name the evidence used;
5. mark unsupported fields `UNKNOWN`;
6. preserve contradictions;
7. identify what requires validation;
8. avoid turning solution ideas into facts.
