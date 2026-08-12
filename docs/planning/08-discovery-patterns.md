# DISCOVER Discovery Patterns

> **Purpose:** Provide reusable starting patterns for common discovery objectives while preserving practitioner judgement.

Patterns are recommendations, not mandatory recipes.

Each pattern should be adapted to:

- business context;
- evidence;
- stakeholder access;
- risk;
- available time;
- discovery maturity.

---

# Pattern 1 — Understand a Business Domain

## Typical Request

> "I need to understand Finance."

## Primary Objective

Build sufficient shared understanding of the domain to identify priority areas for deeper discovery.

## DISCOVER

Primary:

- Define
- Investigate
- Study

Continuous:

- Capture
- Validate

## POPIT-V

Very High:

- Organisation
- Process
- Information
- Value

High:

- People

Medium:

- Technology

## Techniques

- Stakeholder Mapping
- Capability Mapping
- Interviews
- Process Walkthroughs
- Business Glossary

Potential:

- EventStorming
- Ontology Discovery

## Workshops

1. Business Context and Capabilities
2. Processes and Decisions
3. Information, Rules and Terminology
4. Validation / Priorities

## Core Artefacts

- Stakeholder Register
- Capability Map
- Decision Catalogue
- Business Glossary
- Evidence Register
- Golden Thread

## Exit Criteria

The domain is understood well enough to identify where deeper discovery will create value.

---

# Pattern 2 — Improve an Existing Process

## Typical Request

> "Month-end is too slow."

## Primary Objective

Establish where and why flow is constrained and identify evidence-based improvement opportunities.

## DISCOVER

- Define
- Study
- Capture
- Validate
- Evaluate

## POPIT-V

Very High:

- Process

High:

- People
- Information
- Value

Medium:

- Organisation
- Technology

## Techniques

- Process Modelling
- Value Stream Mapping
- Observation
- Decision Catalogue
- Data / evidence review

## Questions

- What triggers the process?
- What is the outcome?
- Where does work wait?
- What causes rework?
- Which decisions/approvals matter?
- Which information arrives late?
- Which exceptions dominate?
- What is the measurable impact?

## Artefacts

- Process Map
- Pain Point Register
- Evidence Register
- Decision Catalogue
- Benefits / Value Register

## Exit Criteria

Material constraints and root-cause hypotheses are sufficiently evidenced to evaluate interventions.

---

# Pattern 3 — Resolve Reporting / Metric Conflict

## Typical Request

> "Different dashboards show different numbers."

## Objective

Determine whether disagreement results from semantics, rules, sources, timing, transformation or context.

## POPIT-V

Very High:

- Information

High:

- Process
- Organisation

Medium:

- Technology
- Value

## Techniques

- Business Glossary
- KPI Catalogue
- Report Review
- Business Rules Catalogue
- Lineage Review

## Questions

- What decision does each report support?
- How is the metric defined?
- What is included/excluded?
- What time period/grain is used?
- Which rule is applied?
- Which source and transformation is used?
- Are both values valid in different contexts?

## Artefacts

- KPI Catalogue
- Business Glossary
- Business Rules Catalogue
- Evidence Register
- Data Catalogue / lineage

## Exit Criteria

The cause of disagreement is understood and semantic/governance decisions are explicit.

---

# Pattern 4 — Design a Data Product

## Typical Request

> "We need a Finance data product."

## Objective

Determine whether a coherent product exists and define the consumer, decision, information, service and value.

## DISCOVER

- Define
- Study
- Organise
- Validate
- Evaluate

## POPIT-V

Very High:

- Information
- Value

High:

- People
- Process
- Organisation

Medium:

- Technology initially

## Questions

- Who is the consumer?
- Which decision/action is supported?
- Which business concepts are required?
- What quality/freshness is needed?
- Who owns the product?
- Who owns the data?
- What service expectation exists?
- What measurable value is expected?

## Artefacts

- Data Product Canvas
- Decision Catalogue
- Business Glossary
- Data Catalogue
- Benefits / Value Register
- Golden Thread

## Exit Criteria

A validated product hypothesis exists, or evidence shows a product is not the right intervention.

---

# Pattern 5 — Identify AI Opportunities

## Typical Request

> "Where could Finance use AI?"

## Objective

Identify tasks/decisions where AI could create incremental business value with acceptable risk.

## DISCOVER

- Define
- Investigate
- Study
- Evaluate

## POPIT-V

Very High:

- People
- Process
- Information
- Value

High:

- Organisation
- Technology

## Techniques

- Process / task analysis
- Decision Catalogue
- AI Opportunity Canvas
- Information / data assessment
- risk assessment

## Questions

- Which task consumes judgement or repetitive effort?
- Which decision would improve?
- What information would AI require?
- What must remain human-controlled?
- How would output quality be evaluated?
- What could go wrong?
- What non-AI intervention could solve the same problem?
- What value would successful AI create?

## Artefacts

- AI Opportunity Canvas
- Decision Catalogue
- Risk Register
- Evidence Register
- Benefits / Value Register

## Exit Criteria

A small number of evidence-based AI hypotheses are ready for evaluation/experiment, or AI has been ruled out.

---

# Pattern 6 — Build a Business Ontology

## Typical Request

> "We need an ontology for Finance."

## Objective

Create validated business semantics that answer relevant competency questions and can be mapped to data.

## DISCOVER

- Define
- Study
- Capture
- Organise
- Validate

## POPIT-V

Very High:

- Information

High:

- Organisation
- Process
- People
- Value

Medium:

- Technology

## Techniques

- Business Glossary
- Ontology Discovery
- Domain-Driven Design
- EventStorming where helpful
- source mapping after semantics are understood

## Questions

- What business questions must the ontology support?
- What are the important concepts?
- How are they defined?
- How are they related?
- Which rules constrain relationships?
- Where does meaning change by context?
- Who owns each concept?
- Which data sources represent the concepts?

## Artefacts

- Competency Question Catalogue
- Business Glossary
- Ontology Capture
- Business Rules Catalogue
- Source-to-Concept Mapping
- Evidence Register

## Exit Criteria

The semantic model can answer the priority competency questions and has ownership/governance.

---

# Pattern 7 — Assess Data Quality

## Typical Request

> "Our Finance data quality is poor."

## Objective

Determine whether specific data-quality problems materially affect business decisions or outcomes.

## POPIT-V

Very High:

- Information

High:

- Process
- Value

Medium:

- People
- Technology
- Organisation

## Techniques

- Decision analysis
- Data profiling
- Process walkthrough
- lineage review
- Business Rules Catalogue

## Questions

- Which decision is affected?
- What does "poor quality" mean here?
- Which quality dimension fails?
- What threshold is required?
- Where is the issue introduced?
- Where is it detected?
- What business impact results?
- Is the issue semantic rather than physical?

## Artefacts

- Data Catalogue
- quality requirements
- Evidence Register
- Pain Point Register
- Business Rules Catalogue

## Exit Criteria

Quality problems are defined in business context with measurable requirements and probable causes.

---

# Pattern 8 — Rationalise Reporting

## Typical Request

> "We have too many Finance reports."

## Objective

Determine which reports are valuable, duplicated, obsolete or semantically inconsistent.

## POPIT-V

Very High:

- Information
- Value

High:

- People
- Process

Medium:

- Organisation
- Technology

## Techniques

- report inventory;
- usage analysis;
- Decision Catalogue;
- KPI Catalogue;
- interviews.

## Questions

- Who uses the report?
- Which decision/action does it support?
- How often is it used?
- Which measures does it contain?
- Is the definition duplicated elsewhere?
- What manual effort produces it?
- What happens if it is retired?

## Artefacts

- Report Inventory
- KPI Catalogue
- Decision Catalogue
- Opportunity Register
- Benefits / Value Register

## Exit Criteria

Reports can be classified into retain, improve, consolidate, replace or retire with evidence.

---

# Pattern 9 — Establish Governance

## Typical Request

> "Nobody knows who owns the data."

## Objective

Clarify ownership, decision rights and governance for important business information or products.

## POPIT-V

Very High:

- Organisation
- People

High:

- Information

Supporting:

- Process
- Value
- Technology

## Techniques

- Stakeholder Mapping
- RACI / responsibility analysis
- Capability Mapping
- glossary/data ownership review
- governance workshop

## Questions

- Who owns the business concept?
- Who can approve a definition change?
- Who maintains the physical data?
- Who owns quality?
- Which forum resolves disputes?
- What authority does ownership include?
- How is change governed?

## Artefacts

- RACI
- Stakeholder Register
- ownership register
- Business Glossary
- governance model

## Exit Criteria

Ownership and decision rights are explicit enough for operational governance.

---

# Pattern 10 — Modernise Legacy Technology

## Typical Request

> "We need to replace the Finance platform."

## Objective

Understand the business capabilities, processes, information and constraints that any future technology must support.

## POPIT-V

Very High:

- Process
- Information
- Technology

High:

- Organisation
- People
- Value

## Techniques

- Capability Mapping
- Process Modelling
- Business Glossary
- system/integration mapping
- technical constraint assessment

## Questions

- Which capabilities depend on the platform?
- Which processes are constrained?
- Which business rules are embedded?
- Which information is mastered?
- Which workarounds exist?
- What must future technology enable?
- What value is expected from change?

## Artefacts

- Capability Map
- Process Maps
- Business Rules Catalogue
- Information model
- Technology Landscape
- Benefits / Value Register

## Exit Criteria

Future-state requirements are expressed as business capabilities/outcomes rather than current-system features.

---

# Using Patterns

When a request matches a pattern:

1. state the inferred objective;
2. explain the pattern selected;
3. adapt it to the domain/context;
4. ask clarifying questions only where they materially alter the plan;
5. generate the workshop/questions/evidence;
6. define exit criteria;
7. recommend what comes next.

Do not present the pattern as mandatory.

---

# Pattern Combination

Complex engagements may combine patterns.

Example:

Finance domain discovery may begin with:

**Understand a Business Domain**

then branch into:

- Improve an Existing Process;
- Resolve Reporting Conflict;
- Build an Ontology;
- Design a Data Product;
- Identify AI Opportunities.

The practitioner should sequence patterns based on evidence and value.

---

# Pattern Selection Test

Before using a pattern ask:

- Does it match the primary objective?
- Does the user already know enough to use a more focused pattern?
- What uncertainty does it address?
- What evidence will it produce?
- What would cause us to change pattern?

Patterns are starting points for reasoning, not recipes.
