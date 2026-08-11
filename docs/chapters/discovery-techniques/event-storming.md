---
title: "EventStorming"
version: "1.2"
status: "Practitioner Technique"
---

# EventStorming

> *"The primary output is not the wall of sticky notes; it is the shared understanding created while building it."*

## Purpose

EventStorming is a collaborative modelling technique created by Alberto Brandolini for exploring complex business domains through significant **domain events**.

It is particularly effective when several groups hold different parts of the truth and the discovery team needs to learn quickly.

## Why This Matters

Traditional interviews can produce separate narratives that are difficult to reconcile.

EventStorming brings domain experts and practitioners together around a shared timeline. It makes visible:

- business events;
- triggers and commands;
- decisions;
- policies;
- actors;
- external systems;
- hotspots;
- exceptions;
- terminology;
- candidate bounded contexts.

It is a form of **deliberate collective learning** rather than simply process documentation.

## What Is a Domain Event?

A domain event is something meaningful that **has happened** in the business.

Write events in past tense, for example:

- Contract Signed
- Right Acquired
- Licence Approved
- Revenue Recognised
- Forecast Submitted
- Campaign Launched

Avoid technical events such as:

- Row Inserted
- API Called

unless the technical event itself is meaningful to the business question.

## Common EventStorming Elements

Different workshop styles use different colour conventions. DISCOVER is interested in the concepts rather than enforcing colours.

Potential elements:

- Domain Event;
- Command / Trigger;
- Actor;
- Policy / Business Rule;
- Read Model / Information;
- External System;
- Aggregate / Business Concept;
- Hotspot;
- Opportunity;
- Question.

## How It Fits DISCOVER

EventStorming is useful during:

- Investigate;
- Study;
- Capture;
- Organise;
- Validate.

It can reveal material for:

- Process Models;
- Decision Catalogue;
- Business Rules Catalogue;
- Business Glossary;
- Ontology;
- Bounded Contexts;
- Pain Point Register.

## When to Use It

Use when:

- the domain is complex;
- several teams need shared understanding;
- the process is poorly documented;
- terminology differs;
- exceptions matter;
- integration boundaries are unclear;
- you need rapid discovery before detailed modelling.

## When Not to Use It

Avoid a large EventStorming workshop when:

- the problem can be solved with a focused interview;
- participants cannot safely discuss the domain together;
- the required evidence is primarily documentary;
- the session objective is too vague.

## Workshop Preparation

### Participants

Include:

- domain experts;
- people who perform the work;
- decision makers where useful;
- analysts/facilitators;
- technical specialists only where they help answer domain questions.

Do not fill the room only with delivery/technology staff.

### Scope

Define:

- business question;
- start/end boundaries;
- timebox;
- expected outputs.

### Physical / Digital Space

Provide enough space for a long timeline. The visual nature of the technique is important.

## Big Picture EventStorming

### Step 1 — Storm the Events

Participants independently add significant business events.

Encourage breadth.

### Step 2 — Establish Rough Time Order

Arrange events left to right.

Do not obsess about perfect sequence immediately.

### Step 3 — Find Hotspots

Mark:

- disagreement;
- missing knowledge;
- pain;
- uncertainty;
- risk;
- exceptions.

Hotspots are valuable discovery outputs.

### Step 4 — Add Actors and Triggers

Ask:

- Who caused this?
- What decision or command caused it?
- What information did they need?

### Step 5 — Add Policies / Rules

Ask:

- What makes the next thing happen?
- Which rule decides the path?
- Who can override it?

### Step 6 — Add External Systems / Parties

Only after the domain behaviour is understood enough.

### Step 7 — Identify Language and Boundaries

Look for:

- terms that change meaning;
- ownership boundaries;
- clusters of events;
- candidate bounded contexts.

### Step 8 — Capture Follow-Up

Convert hotspots into:

- Open Questions;
- Evidence requests;
- Decision Catalogue entries;
- Business Rules;
- Process hypotheses;
- Ontology concepts.

## Questions During the Session

- What happened?
- What caused that event?
- Who initiated it?
- What information did they have?
- What rule was applied?
- What happens if the normal path fails?
- Can the event happen twice?
- Can events occur in a different order?
- Who needs to know the event occurred?
- What changes as a result?
- Which event represents real business value?

## Finance Example

A revenue-recognition EventStorm might include:

Contract Signed → Delivery Obligation Met → Recognition Assessed → Adjustment Approved → Revenue Recognised → Revenue Reported

Hotspots may expose:

- disagreement about the recognition trigger;
- reliance on contract wording;
- manual adjustment;
- unclear ownership;
- differences between sales and accounting terminology.

The next step is not “build an event-driven architecture”. The events first help understand the business.

## Marketing Example

Campaign Brief Approved → Audience Selected → Media Booked → Campaign Activated → Response Recorded → Performance Reviewed → Budget Reallocated

Hotspots might reveal:

- campaign IDs do not persist across platforms;
- attribution rules differ;
- agency data arrives too late;
- optimisation decisions are informal.

## EventStorming and DDD

EventStorming is strongly associated with Domain-Driven Design because it can surface:

- ubiquitous language;
- domain events;
- aggregates;
- subdomains;
- bounded contexts;
- context boundaries.

However, DISCOVER can use EventStorming without committing to a software architecture.

## EventStorming and the Golden Thread

Events can help connect:

- process;
- decision;
- information;
- business rule;
- action;
- value.

A significant domain event may also become an important data concept or event contract later—but only after validation and design.

## Outputs

- Event Timeline;
- Hotspot Register;
- Domain Vocabulary;
- Decision hypotheses;
- Business Rule hypotheses;
- Process model inputs;
- Context/Domain boundaries;
- Open Questions;
- Opportunity hypotheses.

## Common Pitfalls

- treating sticky colours as more important than learning;
- inviting only technical staff;
- turning the session into solution architecture;
- using technical event names;
- skipping exceptions;
- trying to “clean up” disagreements during the workshop;
- failing to convert hotspots into structured follow-up;
- assuming events discovered in one session are complete.

## Facilitation Tips

- keep participants standing/moving where possible;
- use silent contribution before group debate;
- timebox debates and mark hotspots;
- encourage past-tense event names;
- ask for concrete examples;
- capture contradictions visibly;
- photograph/export the board before restructuring it.

## Practitioner Checklist

- [ ] Scope is clear.
- [ ] Domain experts are present.
- [ ] Events are business-meaningful.
- [ ] Hotspots are captured.
- [ ] Decisions, information and rules are explored.
- [ ] Exceptions are visible.
- [ ] Terminology conflicts are preserved.
- [ ] Follow-up evidence is assigned.
- [ ] Outputs are transferred into reusable DISCOVER artefacts.

## References

- Brandolini, A., *Introducing EventStorming: An Act of Deliberate Collective Learning*. Leanpub.
- Evans, E. (2003), *Domain-Driven Design*. Addison-Wesley.
- Vernon, V. (2016), *Domain-Driven Design Distilled*. Addison-Wesley.
- EventStorming.com, official resources.

## Chapter Summary

EventStorming accelerates shared learning by making business events, decisions, rules and disagreements visible. In DISCOVER its value lies in exposing the domain, not in prescribing a technical implementation.
