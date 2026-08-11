---
title: "Technology"
chapter: 15
version: "1.2"
status: "Practitioner Reference"
---

# Technology

> *"Technology should explain how the business is enabled or constrained—not define what the business is."*

## Purpose

The **Technology** perspective focuses on the systems, applications, platforms, integrations, spreadsheets, data stores, analytical tools, automation and AI components that currently support the business.

DISCOVER deliberately examines Technology **after** establishing business context. The purpose is to understand enablement, constraints, risks and dependencies—not to let the existing system landscape define the future business model.

## Why This Matters

Technology can:

- automate work;
- enforce rules;
- create and store information;
- connect teams;
- enable analytics;
- improve controls;
- create new capabilities.

It can also create:

- fragmentation;
- manual integration;
- duplicated data;
- hidden logic;
- vendor lock-in;
- technical debt;
- operational risk;
- poor observability;
- constraints that shape business behaviour.

Many organisations mistakenly model their business around application boundaries. DISCOVER keeps durable business concepts separate from transient technology choices.

## Discovery Objectives

Understand:

- applications and platforms;
- business purpose of each;
- system owners;
- users;
- interfaces and integrations;
- data stores;
- spreadsheets and local tools;
- reporting/BI;
- workflow and automation;
- AI components;
- identity/access;
- resilience;
- observability;
- lifecycle and support;
- technical debt;
- cost and licensing;
- planned change;
- constraints affecting business outcomes.

## What Good Looks Like

You should be able to answer:

- Which technologies enable the capability?
- What business purpose does each serve?
- Where is information created and mastered?
- How does information move?
- Where are manual exports/imports used?
- Which spreadsheets are operational dependencies?
- Which business rules are embedded in code?
- What fails frequently or invisibly?
- Which platforms duplicate capability?
- Which technology is near end of life?
- Which constraints materially limit the business?
- Which data/AI opportunities can use existing platforms safely?

## What to Discover

### Applications

Capture:

- application name;
- business purpose;
- capabilities supported;
- owner;
- user groups;
- criticality;
- vendor;
- lifecycle status;
- major constraints.

### Integration

Understand:

- APIs;
- files;
- SFTP;
- queues/events;
- ETL/ELT;
- manual transfer;
- batch timing;
- failure handling;
- reconciliation;
- dependencies.

### Data Platforms

Explore:

- operational databases;
- warehouses/lakehouses;
- semantic layers;
- catalogues;
- data product platforms;
- orchestration;
- quality controls;
- lineage;
- environments;
- access patterns.

### Reporting and Analytics

Identify:

- BI/reporting tools;
- self-service tools;
- analytical notebooks;
- extracts;
- spreadsheets;
- embedded SaaS reporting;
- semantic models;
- duplicated reporting stacks.

### Automation and Workflow

Capture:

- workflow engines;
- RPA;
- scripts;
- scheduled jobs;
- rules engines;
- manual workarounds;
- exception queues.

### AI

Understand:

- existing ML/AI services;
- GenAI/LLM components;
- agents;
- retrieval systems;
- model providers;
- evaluation;
- governance;
- human oversight;
- data access;
- monitoring.

Do not treat “AI” as one technology category. Understand the concrete capability and risk.

### Security and Access

Explore:

- identity;
- authentication;
- authorisation;
- least privilege;
- data sensitivity;
- segregation of duties;
- audit;
- privileged access;
- external sharing.

### Reliability and Operations

Capture:

- critical SLAs/SLOs;
- monitoring;
- alerting;
- incident patterns;
- recovery;
- support model;
- manual restart;
- dependency on key people.

### Lifecycle and Technical Debt

Understand:

- end-of-life systems;
- unsupported components;
- brittle integrations;
- duplicated tools;
- customisation;
- upgrade blockers;
- backlog;
- data migration dependencies.

## Generic Discovery Questions

### Applications

- Which systems are essential to this activity?
- What business capability does each support?
- Who owns the application?
- What would happen if it were unavailable?
- Which features are not used?
- Where do users leave the system to complete the work?

### Integration

- How does information enter and leave?
- Is transfer real-time, batch or manual?
- What happens when the integration fails?
- How is completeness checked?
- Where are files downloaded and re-uploaded?
- Which reconciliations exist because systems disagree?

### Data and Reporting

- Where is the underlying data stored?
- Which datasets are reused?
- Is there a governed semantic layer?
- Which reports bypass the central data platform?
- Which transformations contain business logic?
- Where is lineage unavailable?

### Spreadsheets

- Which spreadsheets are business critical?
- What rules do they implement?
- Who maintains them?
- How are versions controlled?
- What breaks if the author is unavailable?

Spreadsheets are not inherently bad; hidden ownership and uncontrolled critical logic are the risk.

### Reliability

- Which failures occur repeatedly?
- How are they detected?
- Who is alerted?
- What requires manual recovery?
- What is the business impact of downtime or stale data?

### Constraints

- Which technology limits the business today?
- Which constraint is contractual rather than technical?
- Which systems are due to change?
- Which dependencies make change risky?
- Which planned programme could invalidate today's design?

### AI and Automation

- Which user task would be improved?
- What information can the component access?
- How will outputs be evaluated?
- What must remain human-controlled?
- How is sensitive information protected?
- What happens when the model is wrong?


## Evidence to Capture

Do not treat workshop conversation as automatically validated fact. Capture important findings using the DISCOVER evidence model:

- **Evidence** — explicitly supported by a trusted source, observed artefact or validated record.
- **Stakeholder Statement** — stated by a stakeholder but not yet independently validated.
- **Assumption** — plausible but unverified.
- **Interpretation** — an analytical conclusion drawn from evidence.
- **Recommendation** — a proposed intervention.
- **Open Question** — information still required.

Where evidence conflicts, record the contradiction and identify who or what can validate it. Use `UNKNOWN` when an important Golden Thread link is not established.


## Technology Is Not the Business Model

Avoid statements such as:

- “Salesforce owns Customer.”
- “Rightsline is Rights.”
- “BigQuery is the ontology.”
- “The spreadsheet is the forecast process.”

Instead:

- model the business concept or capability independently;
- then map the technology that currently represents or supports it.

This makes the discovery resilient to future platform change.

## Discovery Artefacts

- Systems Landscape;
- Application Catalogue;
- Integration Map;
- Data Source Catalogue;
- Technology Dependency Map;
- System-to-Capability Mapping;
- Technical Constraint Register;
- Technology Risk Register;
- Data Lineage;
- AI Component Register;
- Golden Thread Traceability.

## Typical Pain Points

- fragmented applications;
- point-to-point integrations;
- manual file transfer;
- spreadsheet dependency;
- duplicated reporting tools;
- hidden business logic;
- low observability;
- stale batch data;
- inconsistent identity/access;
- technical debt;
- unsupported systems;
- duplicated data;
- poor lineage;
- vendor lock-in;
- uncontrolled AI experimentation.

## Opportunities

- rationalise platforms;
- expose reusable APIs/events;
- centralise governed business logic where appropriate;
- improve observability;
- automate reliable repeatable work;
- create shared semantic/data services;
- retire duplicate reporting;
- improve identity and access;
- strengthen lineage;
- modernise integrations;
- introduce governed AI components;
- separate durable business semantics from physical systems.

## Maturity Signals

### Fragmented
Point solutions, manual files, hidden spreadsheets, brittle integrations and reactive support.

### Developing
Shared platforms exist but adoption, integration and governance are uneven.

### Defined
Architecture patterns, ownership, observability and lifecycle management are established.

### Managed
Reliability, cost, quality, security and platform usage are measured; technical debt is actively prioritised.

### Adaptive
Technology is modular, observable and governed; platforms evolve without breaking business semantics; AI and automation are evaluated continuously.

## Finance Example

### Discovery Focus

Understand how ERP/ledger, planning, rights/sales systems, spreadsheets, reporting and data platforms enable forecasting and revenue reporting.

### Questions

- Which system records the contractual fact?
- Which system records the accounting result?
- Where are adjustments made outside systems?
- How is data transferred between commercial and Finance systems?
- Which spreadsheet calculations are critical?
- How are FX, period and chart-of-accounts mappings maintained?
- What is the reporting latency?
- Can a Finance user trace a number to source and rule?

### Opportunities

Potential opportunities might include governed finance data products, automated reconciliation, rule transparency or workflow improvement—but only after business rules and ownership are understood.

## Marketing Example

Explore CRM/CDP, media platforms, ad servers, analytics, social platforms, agency data feeds and BI.

Ask:

- how campaign identifiers persist across tools;
- how audience definitions are transferred;
- where cost and outcome data are joined;
- which platform metrics differ semantically;
- where manual extracts occur;
- how attribution logic is implemented.


## Golden Thread Connection

This perspective should not exist as an isolated checklist. Connect findings to the Golden Thread wherever the evidence supports it:

**Business Strategy → Business Capability → Business Process → Business Decision → Business Information → Business Rules → Technology / Data → Data Product / Analytics → Insight / Action → Business Value**

Use stable identifiers when the engagement requires traceability:

- `STR-` Strategic Objective
- `CAP-` Business Capability
- `PRC-` Business Process
- `DEC-` Business Decision
- `INF-` Information
- `BR-` Business Rule
- `SYS-` System / Technology
- `DAT-` Data Asset
- `DP-` Data Product
- `ACT-` Business Action
- `VAL-` Business Value

Supporting discovery records may use `EVD-`, `ASM-`, `OQ-`, `PAIN-`, `OPP-` and `RSK-`.

The objective is traceability rather than bureaucracy. Do not invent links merely to complete the chain.


## AI Governance Note

Where AI is considered, discovery should include risk and management-system requirements. Relevant reference points include ISO/IEC 42001:2023 and the NIST AI Risk Management Framework. The NIST AI RMF is structured around **Govern, Map, Measure and Manage** and is intended to support risk management rather than act as a simple compliance checklist.

## Facilitation Cautions

- Do not let technology owners define business meaning unchallenged.
- Avoid solution architecture before the business decision and information are understood.
- Separate current constraints from future requirements.
- Do not assume “centralise everything” is the right answer.
- Record planned system changes as dependencies.
- Treat AI output quality, monitoring and human oversight as first-class concerns.

## Practitioner Checklist

- [ ] Business purpose of each critical system is known.
- [ ] System ownership is distinguished from data/business ownership.
- [ ] Critical integrations and manual transfers are visible.
- [ ] Spreadsheet dependencies are captured.
- [ ] Embedded business rules are identified.
- [ ] Reliability/observability concerns are understood.
- [ ] Security/access constraints are captured.
- [ ] Technical debt and lifecycle risks are visible.
- [ ] AI components have governance and evaluation considerations.
- [ ] Technology findings connect to business decisions and value.

## References

- The Open Group, *TOGAF® Standard, 10th Edition*.
- ISO/IEC 27001:2022, *Information security, cybersecurity and privacy protection — Information security management systems — Requirements*.
- ISO/IEC 42001:2023, *Artificial intelligence — Management system*.
- NIST (2023), *Artificial Intelligence Risk Management Framework (AI RMF 1.0)*.
- NIST (2024), *Artificial Intelligence Risk Management Framework: Generative Artificial Intelligence Profile (NIST AI 600-1)*.
- Hohpe, G. & Woolf, B. (2003), *Enterprise Integration Patterns*. Addison-Wesley.
- Forsgren, N., Humble, J. & Kim, G. (2018), *Accelerate*. IT Revolution.

## Chapter Summary

The Technology perspective makes the enabling landscape and its constraints visible without allowing applications to define the business. This creates a safer foundation for architecture, data products, automation and AI because technical choices remain traceable to business decisions and value.
