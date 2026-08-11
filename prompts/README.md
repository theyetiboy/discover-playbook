# DISCOVER Domain Prompt Packs

> Domain prompt packs turn the DISCOVER methodology into practical conversation starters for a source-grounded AI assistant. They are **not domain truth**.

## Available Packs

- `Example-Prompt-Finance.md`
- `Example-Prompt-Rights.md`
- `Example-Prompt-Global-Sales.md`
- `Example-Prompt-Content.md`
- `Example-Prompt-Marketing.md`

## Recommended Notebook Pattern

Load:

1. `core/00-DISCOVER-Core.md`
2. `core/01-Notebook-Operating-Instructions.md`
3. `core/02-Example-Prompt-Template.md`
4. the relevant domain prompt pack;
5. required canonical templates;
6. trusted business evidence.

The domain prompt pack provides **hypotheses and questions**, not answers.

## Prompt Design Rules

A good DISCOVER prompt should:

- state the business area and objective;
- preserve solution neutrality;
- ask the assistant to select relevant DISCOVER stages;
- select only relevant POPIT-V lenses;
- identify Golden Thread links;
- distinguish evidence from inference;
- ask for `UNKNOWN` where sources are silent;
- end with validation / next evidence.

## Example

```text
I am starting discovery with Finance.

The current concern is that forecasting takes too long and users do not
trust the numbers.

Treat those concerns as stakeholder statements rather than established
root causes.

Using DISCOVER:
1. identify the most important business outcomes and decisions to explore;
2. recommend the DISCOVER stages and POPIT-V lenses for an initial workshop;
3. identify the Golden Thread links we need to establish;
4. create a 90-minute workshop;
5. identify evidence we should capture;
6. list assumptions and open questions.

Do not propose a dashboard, platform or AI solution unless the supplied
evidence supports moving to solution evaluation.
```

## After a Workshop

Useful prompt pattern:

```text
Analyse the supplied workshop notes using DISCOVER.

Update the canonical artefacts using existing stable IDs.
Create new IDs only for genuinely new items.

Separate:
- Evidence
- Stakeholder Statement
- Assumption
- Interpretation
- Recommendation
- Open Question

Show Broken Threads and mark unsupported fields UNKNOWN.

Do not resolve contradictions without evidence.
```

## Domain Packs Are Extensible

A domain pack may be expanded for an organisation or initiative, for example:

- Royalties
- Brand Licensing
- Production
- Digital Studios
- HR / People
- Procurement
- Legal / Contracts

Keep organisation-specific facts out of the generic pack. Put those facts in the notebook evidence sources instead.

## Governance

When a generic domain pack changes:

- verify it remains consistent with `docs/methodology/`;
- keep questions neutral;
- avoid embedding vendor assumptions;
- maintain business-before-technology;
- maintain Decisions Drive Data;
- maintain explicit Value.

## Source-Grounded Principle

The assistant can help:

- prepare;
- question;
- structure;
- compare;
- identify gaps.

Only organisational evidence and appropriate stakeholders can establish the organisation's business truth.
