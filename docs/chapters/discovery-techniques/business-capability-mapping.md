---
title: "Business Capability Mapping"
version: "1.0"
author: "Steve Tarry"
technique: "Discovery Technique"
---

# Business Capability Mapping

## Purpose

Business Capability Mapping provides a structured view of **what an organisation must be able to do** in order to achieve its objectives.

It deliberately abstracts away from individual processes, organisational structures and technology implementations. This provides a relatively stable business view that can be used to understand the organisation, assess capability maturity, identify gaps and align investment with strategy.

Business Capability Analysis can support strategic alignment, scoping, planning and prioritisation by establishing a shared understanding of the capabilities required to achieve desired outcomes (IIBA, n.d.).

Within DISCOVER, Capability Mapping is particularly useful during the **Investigate**, **Organise**, **Evaluate** and **Roadmap** stages.

---

# Why This Technique Matters

Discovery frequently begins with existing systems, organisational structures or reports.

This can create a distorted view of the business because:

- Organisation structures change.
- Technology platforms are replaced.
- Processes evolve.
- Responsibilities move between teams.

Business capabilities provide another perspective: the enduring abilities the organisation requires in order to operate and create value.

Capability maps can therefore provide a common business blueprint against which strategy, processes, information, organisation and technology can be assessed (Business Architecture Guild, n.d.).

---

# When to Use Capability Mapping

Capability Mapping is particularly useful when:

- Entering an unfamiliar business domain
- Starting a transformation programme
- Defining a Data & Analytics strategy
- Exploring opportunities for new Data Products
- Assessing AI opportunities
- Reviewing duplicated systems or processes
- Understanding organisational complexity
- Identifying investment priorities
- Creating an enterprise architecture
- Designing an operating model
- Defining a product roadmap

It is often one of the most useful early discovery techniques because it provides a structure into which later findings can be organised.

---

# What is a Business Capability?

A Business Capability describes an ability required by an organisation to achieve an outcome or fulfil its purpose.

Capabilities describe **what the organisation needs to be able to do**, rather than the detailed process through which that ability is delivered.

For example:

```text
Financial Management
```

is a capability.

Whereas:

```text
Finance analyst downloads a spreadsheet,
reconciles transactions,
obtains approval,
and uploads a journal.
```

is describing a process.

Keeping this distinction clear is important.

---

# Capability vs Process

A useful way to distinguish the two is:

| Capability | Process |
|------------|---------|
| What the organisation can do | How work is performed |
| Relatively stable | Changes more frequently |
| Outcome focused | Activity focused |
| Independent of specific technology | Often enabled by specific systems |
| Useful for strategic planning | Useful for operational analysis |

Example:

```text
Capability

Revenue Management
```

may be realised through several processes:

```text
Contract Creation
        ↓
Revenue Recognition
        ↓
Billing
        ↓
Cash Collection
        ↓
Financial Reporting
```

The capability should not be defined by any one of those individual processes.

---

# Capability Hierarchy

Capabilities are commonly organised into levels.

A simple DISCOVER model uses three.

## Level 1 – Business Domain

A broad organisational capability area.

Example:

```text
Finance
```

---

## Level 2 – Capability Group

A logical grouping of related capabilities.

Example:

```text
Financial Planning & Management
```

---

## Level 3 – Business Capability

A more specific business ability.

Example:

```text
Budget Management
Forecasting
Revenue Management
Cost Management
Financial Reporting
```

A capability hierarchy might therefore look like:

```text
Finance
│
├── Financial Planning & Management
│   ├── Budget Management
│   ├── Forecasting
│   └── Scenario Planning
│
├── Revenue Management
│   ├── Revenue Recognition
│   ├── Revenue Attribution
│   └── Revenue Forecasting
│
└── Financial Reporting
    ├── Management Reporting
    ├── Statutory Reporting
    └── Regulatory Reporting
```

The appropriate depth depends upon the purpose of the discovery.

Avoid decomposing capabilities simply because further decomposition is possible.

---

# Capability Naming

Capability names should normally describe an ability using clear business language.

Useful naming patterns include:

```text
Customer Management
Contract Management
Revenue Management
Campaign Management
Rights Management
Content Distribution
Financial Reporting
Audience Measurement
```

Avoid capability names that describe:

### Technology

```text
Salesforce Management
Oracle Reporting
Excel Processing
```

### Organisational Structure

```text
Marketing Team
Finance Department
Data Office
```

### Individual Process Steps

```text
Approve Invoice
Create Spreadsheet
Send Report
```

The capability should describe the business ability independently of how or where it is currently delivered.

---

# Capability Discovery

Capability Mapping should be collaborative.

Useful sources include:

- Business strategy
- Operating models
- Organisation documentation
- Existing process maps
- Products and services
- Stakeholder interviews
- Workshops
- Existing capability models
- Enterprise architecture documentation

Existing documentation provides useful hypotheses, but capabilities should be validated with business stakeholders.

---

# Generic Discovery Questions

## Understanding the Business

- What does this business area exist to achieve?
- What outcomes is it accountable for?
- What services does it provide?
- Who consumes those services?
- What must this area be good at?

---

## Identifying Capabilities

- What must the organisation be able to do to achieve these outcomes?
- Which abilities are essential for the business to operate?
- Which capabilities differentiate the organisation?
- Which capabilities are primarily supporting?
- Which capabilities are required because of regulation or compliance?

---

## Understanding Importance

- Which capabilities are business critical?
- Which capabilities most directly support strategy?
- Which capabilities create competitive advantage?
- Which capabilities would cause significant disruption if they failed?
- Which capabilities are expected to become more important?

---

## Understanding Performance

- Which capabilities perform well today?
- Which capabilities cause frustration?
- Where are there known capability gaps?
- Which capabilities rely heavily on manual work?
- Which capabilities struggle to meet business demand?

---

## Understanding Ownership

- Who owns this capability?
- Who is accountable for its performance?
- Which teams contribute to it?
- Is ownership clear?
- Is the capability duplicated across different areas?

---

## Understanding Information

- What information does this capability require?
- What information does it create?
- Which KPIs measure its performance?
- Which business concepts are central to it?
- What data quality problems affect it?

---

## Understanding Technology

- Which systems enable the capability?
- Are several systems providing the same capability?
- Does existing technology constrain the capability?
- Is any critical activity dependent on spreadsheets or manual workarounds?

---

## Understanding Future Needs

- How will this capability need to change?
- Which strategic initiatives depend upon it?
- What new capabilities will be required?
- Which capabilities require investment?
- Where could Data, Analytics or AI materially improve performance?

---

# Capability Workshop

A typical Capability Mapping workshop may follow this structure.

| Stage | Activity |
|-------|----------|
| 1 | Confirm business purpose and scope |
| 2 | Identify major business outcomes |
| 3 | Identify Level 1 capability areas |
| 4 | Decompose into Level 2 / Level 3 capabilities |
| 5 | Agree definitions |
| 6 | Identify ownership |
| 7 | Assess maturity |
| 8 | Identify pain points |
| 9 | Identify opportunities |
| 10 | Validate the capability map |

The objective is not to create the perfect capability map during the first workshop.

The initial map should be treated as a hypothesis that is progressively validated and refined.

---

# Capability Assessment

Once capabilities have been identified, they can be assessed.

A simple assessment might include:

| Dimension | Score |
|-----------|------:|
| Strategic Importance | 1–5 |
| Business Performance | 1–5 |
| Process Maturity | 1–5 |
| Information Maturity | 1–5 |
| Technology Maturity | 1–5 |
| Data Quality | 1–5 |
| Skills & Knowledge | 1–5 |
| Automation | 1–5 |

The purpose is not to create mathematical precision.

The assessment is intended to expose areas that require further investigation and support prioritisation.

---

# Capability Heatmap

Capabilities may be visualised using a heatmap.

For example:

| Capability | Strategic Importance | Current Maturity |
|------------|---------------------|-----------------|
| Revenue Management | High | Low |
| Financial Reporting | High | Medium |
| Treasury Management | Medium | High |
| Expense Management | Low | High |

This can help identify capabilities where:

```text
High Strategic Importance
            +
Low Current Maturity
            =
Potential Investment Priority
```

Capability analysis can therefore provide a useful input into portfolio prioritisation and transformation planning (IIBA, n.d.).

---

# Connecting Capabilities to POPIT-V

Capabilities should not exist as isolated boxes.

DISCOVER uses the capability as an anchor through which the wider business can be explored.

```text
                     Capability
                         │
          ┌──────────────┼──────────────┐
          │              │              │
       People         Process      Information
          │              │              │
          └──────────────┼──────────────┘
                         │
                    Technology
                         │
                       Value
```

For each capability ask:

### People

- Who owns it?
- Who performs the work?
- What skills are required?

### Organisation

- Which strategic objective does it support?
- Where does accountability sit?

### Process

- Which processes realise the capability?

### Information

- What information does it consume and create?
- Which KPIs measure it?

### Technology

- Which applications and platforms enable it?

### Value

- What business outcome does it deliver?
- What happens if the capability performs poorly?

---

# Connecting Capabilities to DISCOVER Artefacts

Each capability should progressively connect to the wider discovery knowledge base.

```text
Business Strategy
        │
        ▼
Business Capability
        │
        ├──────────────► People
        │
        ├──────────────► Processes
        │
        ├──────────────► Business Information
        │
        ├──────────────► Systems
        │
        ├──────────────► KPIs
        │
        ├──────────────► Data Products
        │
        └──────────────► AI Opportunities
                              │
                              ▼
                        Business Value
```

This traceability is one of the key reasons Capability Mapping is important within DISCOVER.

---

# Finance Example

## Discovery Objective

Understand the capabilities required for the Finance function to provide financial control, planning, reporting and commercial insight.

An initial capability map might identify:

```text
Finance
│
├── Financial Planning & Analysis
│   ├── Budget Management
│   ├── Forecasting
│   ├── Scenario Planning
│   └── Performance Analysis
│
├── Revenue Management
│   ├── Revenue Recognition
│   ├── Revenue Attribution
│   ├── Revenue Forecasting
│   └── Revenue Reconciliation
│
├── Financial Operations
│   ├── Accounts Payable
│   ├── Accounts Receivable
│   ├── Cash Management
│   └── General Ledger Management
│
├── Financial Reporting
│   ├── Management Reporting
│   ├── Statutory Reporting
│   └── Regulatory Reporting
│
└── Financial Governance
    ├── Financial Control
    ├── Audit Support
    └── Compliance Management
```

### Questions

- Which Finance capabilities are considered business critical?
- Which capabilities require significant manual effort?
- Where are spreadsheets used to compensate for missing capabilities?
- Which capabilities rely upon specialist knowledge?
- Which capabilities generate the greatest reporting complexity?
- Where are forecasting and actuals difficult to reconcile?
- Which capabilities depend upon contract or sales information?
- Which capabilities have regulatory or statutory obligations?
- Which areas require better analytics?
- Which capabilities could benefit from AI-supported analysis?

### Potential Findings

Discovery may reveal:

- Revenue Management has high strategic importance but fragmented data.
- Forecasting relies on significant spreadsheet manipulation.
- Financial Reporting contains duplicated reporting activities.
- Revenue Recognition depends upon complex business rules.
- Several capabilities rely upon information from upstream commercial systems.

### Potential Opportunities

These findings could generate opportunities such as:

- Revenue Data Product
- Forecasting Data Product
- Governed Finance Semantic Layer
- Automated Reconciliation
- Financial Commentary Assistant
- Revenue Recognition Rules Catalogue

---

# Marketing Example

## Discovery Objective

Understand the capabilities required to plan, execute, measure and optimise marketing activity.

An initial capability map might identify:

```text
Marketing
│
├── Marketing Strategy
│   ├── Audience Strategy
│   ├── Brand Strategy
│   └── Marketing Planning
│
├── Campaign Management
│   ├── Campaign Planning
│   ├── Campaign Execution
│   └── Campaign Optimisation
│
├── Audience Management
│   ├── Audience Segmentation
│   ├── Audience Targeting
│   └── Customer Insight
│
├── Marketing Performance
│   ├── Campaign Measurement
│   ├── Attribution
│   └── ROI Analysis
│
└── Content Marketing
    ├── Content Planning
    ├── Content Production
    └── Content Distribution
```

### Questions

- Which Marketing capabilities directly support growth?
- Which capabilities differentiate the organisation?
- Which capabilities depend heavily on agencies or third parties?
- How mature is campaign performance measurement?
- Is attribution consistently understood?
- Which capabilities rely upon customer or audience data?
- Where is campaign information fragmented?
- Which capabilities would benefit from better predictive analytics?
- Where could AI reduce manual work?
- Which capabilities require improved integration between Marketing and other functions?

### Potential Findings

Discovery may reveal:

- Campaign Measurement is fragmented across platforms.
- Audience Segmentation uses inconsistent definitions.
- Attribution is calculated differently across teams.
- Campaign optimisation depends upon manually assembled reporting.
- Customer Insight exists across several disconnected datasets.

### Potential Opportunities

These findings could generate:

- Campaign Performance Data Product
- Audience 360
- Marketing Semantic Layer
- Campaign Optimisation Models
- Automated Performance Commentary
- AI Campaign Insight Assistant

---

# Common Pitfalls

## Mapping the Organisation Chart

A capability map should not simply reproduce departments or teams.

Ask:

> "What must the organisation be able to do?"

rather than:

> "Which team does this?"

---

## Mapping Technology

Avoid capabilities such as:

```text
Salesforce Management
Oracle Reporting
Excel Processing
```

These describe technology rather than business ability.

---

## Going Too Deep

Excessive decomposition can make maps unusable.

Only decompose a capability when the additional level provides meaningful analytical value.

---

## Mixing Processes and Capabilities

Activities such as:

```text
Approve Invoice
Create Campaign
Generate Report
```

are usually process activities rather than capabilities.

---

## Treating the Map as Static

Capability maps should evolve as understanding improves.

Discovery may expose missing capabilities, duplicated capabilities or capabilities whose scope needs refinement.

---

# What Good Looks Like

A useful capability map should:

- Be understandable by business stakeholders
- Use business language
- Describe what the organisation can do
- Avoid technology-specific terminology
- Avoid mirroring the organisation chart
- Provide consistent levels of decomposition
- Have clear capability definitions
- Identify ownership where possible
- Support strategic analysis
- Connect to other discovery artefacts

---

# Discovery Outputs

Capability Mapping should contribute to:

- Business Capability Map
- Capability Catalogue
- Capability Definitions
- Capability Ownership
- Capability Maturity Assessment
- Capability Heatmap
- Opportunity Register
- Data Product Opportunities
- AI Opportunities
- Prioritisation
- Roadmap

---

# Related DISCOVER Artefacts

Capability Mapping should link to:

- Discovery Brief
- Stakeholder Register
- Business Glossary
- Process Maps
- Ontology Capture
- Data Catalogue
- KPI Catalogue
- Data Product Canvas
- AI Opportunity Canvas
- Opportunity Register
- Prioritisation Matrix
- Roadmap

---

# Recommended Discovery Questions – Quick Reference

Before completing Capability Mapping, ensure you can answer:

- What does this business area exist to achieve?
- What must it be able to do?
- Which capabilities are business critical?
- Which capabilities support strategy?
- Who owns each capability?
- Which capabilities perform poorly?
- Which capabilities require investment?
- Which information supports them?
- Which technology enables them?
- Which KPIs measure them?
- Which Data Products could improve them?
- Where could AI create value?

---

# References

Business Architecture Guild (n.d.) *Industry Reference Models*. Business Architecture Guild.

Business Architecture Guild (n.d.) *A Guide to the Business Architecture Body of Knowledge (BIZBOK® Guide)*. Business Architecture Guild.

International Institute of Business Analysis (IIBA) (n.d.) *Business Capability Analysis*. In: *A Guide to the Business Analysis Body of Knowledge (BABOK® Guide)*. IIBA.

The Open Group (n.d.) *TOGAF® Series Guides*. The Open Group.

The Open Group (2022) *The TOGAF® Standard, 10th Edition*. Reading, UK: The Open Group.