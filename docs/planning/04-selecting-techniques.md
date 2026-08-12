# Selecting Discovery Techniques

> **Purpose:** Choose the discovery technique that creates the most useful evidence for the current uncertainty.

---

# 1. Techniques Are Tools

DISCOVER techniques are not mandatory stages.

A practitioner should not ask:

> "Which techniques have I not used yet?"

Instead ask:

> **"What do I need to understand, and which technique will help me learn it most efficiently?"**

---

# 2. Technique Selection Criteria

Consider:

- discovery objective;
- uncertainty;
- stakeholder availability;
- complexity;
- evidence already available;
- time;
- need for collaboration;
- need for formal representation;
- expected reuse.

---

# 3. Stakeholder Mapping

Use when you need to understand:

- ownership;
- influence;
- knowledge;
- impacted roles;
- missing perspectives.

Good for:

- unfamiliar domains;
- cross-functional work;
- validation planning.

Do not use it merely to create a communication list.

---

# 4. Business Capability Mapping

Use when you need to understand:

- what the organisation must be able to do;
- domain structure;
- ownership;
- strategic alignment;
- capability maturity.

Good for:

- domain orientation;
- portfolio planning;
- complex organisation structures.

Avoid using teams or systems as capability names.

---

# 5. Structured Interviews

Use when:

- one stakeholder holds specialised knowledge;
- sensitive subjects are involved;
- you need depth;
- participants cannot attend a workshop together.

Good for:

- executive context;
- specialist rules;
- validation;
- conflicting perspectives.

Risk:

Separate interviews can create multiple unconnected narratives.

---

# 6. Process Walkthrough / Process Modelling

Use when you need to understand:

- flow;
- decisions;
- hand-offs;
- exceptions;
- controls;
- operational pain.

Good for:

- slow processes;
- manual work;
- reconciliation;
- unclear ownership.

Do not model more detail than the discovery question requires.

---

# 7. Value Stream Mapping

Use when the problem concerns:

- end-to-end delay;
- queues;
- waiting;
- rework;
- flow efficiency.

Good for:

- month-end close;
- data request flows;
- approval processes.

Requires evidence for timings.

Do not invent measures.

---

# 8. EventStorming

Use when:

- domain is complex;
- multiple teams hold partial knowledge;
- business events are important;
- terminology is inconsistent;
- boundaries are unclear.

Good for:

- rapid shared learning;
- domain exploration;
- discovering decisions/rules/events.

Do not turn the workshop into software architecture.

---

# 9. Business Glossary

Use when:

- important terms conflict;
- KPIs differ;
- multiple teams interpret concepts differently;
- data products need reusable meaning.

Good for:

- Finance;
- Rights;
- Sales;
- Marketing;
- cross-domain data.

Do not start by documenting every noun in the organisation.

---

# 10. Domain-Driven Design

Use strategic DDD concepts when:

- terminology changes by context;
- domains/subdomains are unclear;
- data product boundaries need thought;
- one global model would erase legitimate differences.

Good for:

- bounded contexts;
- ubiquitous language;
- domain ownership.

Do not force software tactical patterns into business discovery.

---

# 11. Ontology Discovery

Use when:

- concepts need explicit relationships;
- cross-domain semantics matter;
- AI/semantic search requires shared meaning;
- a knowledge graph is being considered;
- business questions need reusable semantic structure.

Start with competency questions.

Do not start with RDF/OWL or source schemas.

---

# 12. Wardley Mapping

Use when:

- strategic build/buy decisions matter;
- differentiation vs commodity matters;
- platform dependencies are important;
- future evolution affects direction.

Do not use it for ordinary process discovery.

---

# 13. Data / Report Review

Use when:

- stakeholder claims can be tested against operational evidence;
- reporting duplication is suspected;
- quality/freshness issues matter;
- current metrics need understanding.

Potential activities:

- report inventory;
- KPI comparison;
- field profiling;
- lineage review;
- usage analysis.

Data review complements business discovery. It does not replace it.

---

# 14. Observation / Shadowing

Use when:

- documented process differs from reality;
- manual workarounds matter;
- tacit knowledge is high;
- task friction is difficult to explain verbally.

Ask:

> "Can you show me how you actually do this?"

This can reveal more than another interview.

---

# 15. Technique Selection Matrix

| Discovery Need | Primary Technique | Supporting Techniques |
|---|---|---|
| Understand unfamiliar domain | Capability Mapping | Stakeholder Mapping, Interviews |
| Understand complex workflow | Process Modelling | EventStorming |
| Diagnose delay | Value Stream Mapping | Process Walkthrough |
| Resolve terminology | Business Glossary | Ontology Discovery, DDD |
| Model business semantics | Ontology Discovery | Glossary, DDD |
| Find ownership gaps | Stakeholder Mapping | Capability Mapping |
| Understand events / rules | EventStorming | Process Modelling |
| Assess strategic landscape | Wardley Mapping | Capability Mapping |
| Investigate report conflict | Report Review | Glossary, Decision Catalogue |
| Understand real work | Observation | Interviews, Process Walkthrough |

---

# 16. Combining Techniques

Techniques frequently work together.

Example — Finance Domain:

```text
Stakeholder Mapping
        ↓
Capability Mapping
        ↓
Process Walkthrough
        ↓
Decision Catalogue
        ↓
Business Glossary
        ↓
Ontology Discovery (if justified)
```

Do not interpret the sequence as mandatory.

Let evidence determine what comes next.

---

# 17. Technique Escalation

Start with the simplest technique that can answer the question.

Example:

Terminology problem:

1. Interview / document review.
2. Business Glossary workshop.
3. Concept model.
4. Ontology Discovery.
5. Formal semantic implementation.

Do not jump from "people use different words" to "we need a knowledge graph."

---

# 18. Technique Recommendation Format

When recommending a technique, explain:

## Technique

Capability Mapping

## Why

The domain boundary and business abilities are not understood.

## Evidence Expected

- capability names;
- definitions;
- ownership;
- dependencies.

## Artefacts Updated

- Capability Map;
- Evidence Register;
- Golden Thread.

## Exit Test

The group can explain the major business abilities without referencing the org chart or systems.

---

# 19. Technique Selection Checklist

- [ ] Technique addresses an explicit uncertainty.
- [ ] Existing evidence considered first.
- [ ] Technique is proportionate.
- [ ] Participants are appropriate.
- [ ] Expected evidence is clear.
- [ ] Artefact destination is clear.
- [ ] Exit test exists.
- [ ] Technique does not assume a solution.
