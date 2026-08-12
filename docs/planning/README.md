# DISCOVER Planning

> **Purpose:** Teach practitioners and source-grounded AI assistants how to decide **what discovery to do next, why it matters, and when enough understanding has been achieved.**

The `docs/planning/` section sits between the canonical DISCOVER methodology and the detailed practitioner chapters.

It answers a different question.

The methodology explains:

> **What is DISCOVER?**

The planning section explains:

> **Given the situation in front of me, how should I apply DISCOVER?**

---

# 1. Role of the Planning Layer

The planning layer translates a discovery objective into a proportionate approach.

It helps determine:

- which DISCOVER stages to emphasise;
- which POPIT-V perspectives matter most;
- which techniques are appropriate;
- which stakeholders should be involved;
- which workshops or interviews to run;
- which questions are worth asking;
- which artefacts should be updated;
- which evidence is required;
- what sufficient confidence looks like;
- what should happen next.

It should **reduce unnecessary discovery**, not create more process.

---

# 2. Planning Principle

> **The Planning Layer does not tell the practitioner what to think. It helps the practitioner decide what they need to understand next.**

Every recommendation should therefore be traceable to a discovery objective or uncertainty.

Do not recommend a workshop, technique, question or artefact simply because it exists in the playbook.

---

# 3. Planning Flow

```text
Business Situation
        ↓
Discovery Objective
        ↓
Key Uncertainties
        ↓
Recommended DISCOVER Stages
        ↓
Recommended POPIT-V Perspectives
        ↓
Recommended Techniques
        ↓
Recommended Workshops / Interviews
        ↓
Questions to Ask
        ↓
Evidence to Capture
        ↓
Artefacts to Update
        ↓
Validation / Exit Criteria
        ↓
Next Discovery Activity
```

---

# 4. Files in This Section

## `discovery-planning-guide.md`

The initial planning guide and first planning pattern for **Understand a Business Domain**.

Use it as the high-level entry point.

## `01-applying-discover.md`

Explains how to translate an ambiguous business request into a DISCOVER approach.

## `02-planning-discovery.md`

Provides the detailed planning workflow and the minimum information needed before recommending workshops.

## `03-selecting-popit-v.md`

Explains how to select and weight POPIT-V perspectives rather than applying all six mechanically.

## `04-selecting-techniques.md`

Explains how to choose the technique that will reduce the current uncertainty most efficiently.

## `05-planning-workshops.md`

Explains how to convert the discovery plan into one or more purposeful workshops.

## `06-selecting-artefacts.md`

Explains how to choose only the artefacts needed to preserve and validate learning.

## `07-practitioner-thinking.md`

Captures the judgement patterns used by experienced discovery practitioners.

## `08-discovery-patterns.md`

Provides reusable planning patterns for common objectives such as understanding a domain, improving a process, designing a data product, exploring AI and building an ontology.

---

# 5. Relationship to the Canonical Methodology

`docs/methodology/` remains authoritative.

The planning layer must remain consistent with the following principles:

- Business Before Technology
- Start With Outcomes
- Decisions Drive Data
- Model the Business, Not the Systems
- Evidence Over Assumption
- Explore Before You Converge
- Remain Solution Neutral
- Validate Continuously
- Every Recommendation Must Deliver Value

If a planning recommendation conflicts with the canonical methodology, the canonical methodology wins.

---

# 6. How an AI Assistant Should Use This Section

When a user asks:

> "I need to run a workshop with Finance to understand their domain. What should I do?"

Do **not** immediately return a generic list of POPIT-V questions.

Instead:

1. infer or clarify the discovery objective;
2. identify the important uncertainties;
3. recommend the relevant DISCOVER stages;
4. select and explain the priority POPIT-V lenses;
5. recommend the minimum useful techniques;
6. propose a workshop sequence;
7. explain why each workshop exists;
8. generate questions grouped by the selected perspectives;
9. state what evidence each group of questions is intended to uncover;
10. identify which artefacts should be updated;
11. define exit criteria;
12. recommend the next discovery activity.

If essential planning information is missing, ask only the questions required to materially change the plan.

---

# 7. Standard Planning Response

Where appropriate, use the following structure:

```text
Discovery Objective

Recommended Approach

Recommended DISCOVER Stages

Recommended POPIT-V Focus
- Perspective
- Why it matters
- What we are trying to discover

Recommended Techniques

Workshop Sequence

For Each Workshop / Perspective
- Purpose
- Questions
- Evidence to Capture
- Artefacts to Update
- Exit Criteria

Cross-Cutting Assumptions / Open Questions

Recommended Next Step
```

This response pattern should make the reasoning visible to the practitioner.

---

# 8. What This Section Should Prevent

The planning layer should actively prevent:

- automatically running a six-part POPIT-V workshop;
- asking questions without knowing why;
- completing templates for their own sake;
- jumping to systems before understanding the business;
- treating stakeholder statements as evidence;
- assuming a dashboard, platform, data product or AI solution is required;
- running one enormous workshop when focused sessions would produce better evidence;
- continuing discovery indefinitely when sufficient confidence has been achieved.

---

# 9. Planning Quality Test

Before accepting a discovery plan, ask:

- Is the objective explicit?
- Is every recommended activity linked to an uncertainty?
- Are the POPIT-V lenses selected rather than defaulted?
- Are techniques being used for a clear reason?
- Is the proposed workshop sequence proportionate?
- Does every question have a purpose?
- Is the evidence to capture clear?
- Are outputs reusable?
- Are exit criteria defined?
- Is the next decision or activity clear?

If not, refine the plan.
