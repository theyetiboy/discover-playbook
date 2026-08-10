---
title: "Wardley Mapping"
version: "1.0"
author: "Steve Tarry"
technique: "Discovery Technique"
---

# Wardley Mapping

## Purpose

Wardley Mapping is a strategic mapping technique used to improve situational awareness by visualising the components required to satisfy user needs, the dependencies between those components and their relative stage of evolution.

A Wardley Map combines two important perspectives:

```text
VERTICAL AXIS

Visibility / dependency relative to the user

        +

HORIZONTAL AXIS

Evolution from novel to industrialised
```

The resulting map allows practitioners to explore not only:

> **What exists?**

but also:

> **Where is it positioned, how mature is it, what does it depend upon, and how might it change?**

Wardley Mapping was developed by Simon Wardley as a way of creating greater situational awareness for business strategy (Wardley, 2016–2018).

Within DISCOVER, Wardley Mapping is used primarily as a **strategic discovery and sense-making technique**.

It can help practitioners:

- Understand the landscape surrounding a business problem
- Identify user needs
- Understand dependencies
- Assess how evolved different capabilities are
- Identify inappropriate technology or delivery approaches
- Expose duplication
- Identify strategic constraints
- Explore build, buy or consume decisions
- Understand potential future movement
- Identify investment opportunities
- Explore Data and AI strategy
- Support prioritisation and roadmapping

Wardley Mapping is particularly useful during the **Investigate**, **Study**, **Evaluate** and **Roadmap** stages of DISCOVER.

---

# Why This Technique Matters

Many organisational diagrams show components but provide little strategic context.

For example:

```text
CRM

Finance Platform

Data Warehouse

Reporting Platform

AI Platform
```

may tell us what technology exists.

It does not necessarily tell us:

```text
Why it exists

Who needs it

What it depends upon

How mature it is

Whether it differentiates the organisation

Whether it should be built internally

Whether it is likely to change

Where investment should be concentrated
```

Wardley Mapping introduces **position and movement** into the analysis.

Wardley argues that strategic decision-making benefits from understanding the landscape in which decisions are being made rather than moving directly from organisational purpose to action (Wardley, 2016–2018).

The map therefore provides a shared visual context within which assumptions and strategic choices can be challenged.

---

# What is a Wardley Map?

A Wardley Map begins with a user and their needs.

Those needs depend upon components.

Those components may themselves depend upon other components.

For example:

```text
                         User
                          │
                          ▼
                    Business Insight
                          │
                    ┌─────┴─────┐
                    ▼           ▼
                 Analytics    Business Data
                                  │
                           ┌──────┴──────┐
                           ▼             ▼
                      Data Platform   Source Systems
                                         │
                                         ▼
                                    Infrastructure
```

This creates a **value chain or chain of needs**.

The components are then positioned horizontally according to their stage of evolution.

A simplified Wardley Map might therefore look like:

```text
VISIBLE
TO USER

   User
     │
     ▼
   Insight
      \
       \
        Analytics
              \
               \
                Data Platform
                       \
                        \
                         Compute

─────────────────────────────────────────────────────►

Genesis      Custom Built       Product       Commodity
                                             / Utility

LESS
VISIBLE
TO USER
```

The position of each component is significant.

---

# The Two Axes

A Wardley Map has two primary dimensions.

---

# Vertical Axis – Visibility

The vertical axis represents how visible a component is relative to the user's need.

At the top:

```text
User

User Need
```

Below this are the components required to meet that need.

Components lower in the map generally support components above them.

For example:

```text
User
 │
 ▼
Analytics
 │
 ▼
Data
 │
 ▼
Data Platform
 │
 ▼
Compute
```

The vertical position therefore helps communicate the chain of dependency.

It should not be interpreted simply as organisational importance.

---

# Horizontal Axis – Evolution

The horizontal axis represents how evolved a component is.

The classic Wardley model describes four broad stages:

```text
Genesis
    │
    ▼
Custom Built
    │
    ▼
Product
    │
    ▼
Commodity / Utility
```

Wardley describes evolution as movement driven by competition and supply-and-demand forces, with components tending to move from uncertain and novel forms towards increasingly standardised and industrialised forms (Wardley, 2016–2018).

The stages should be treated as a way of reasoning about context rather than as precise numerical measurements.

---

# Stage 1 – Genesis

Genesis represents the emergence of something new.

Characteristics may include:

```text
Novel

Rare

Poorly understood

Uncertain

Rapid experimentation

High failure

No established market

Unclear best practice
```

Examples might include genuinely new business models, technologies or techniques whose practical use is still being explored.

The key question is:

> **Are we genuinely discovering something new?**

Genesis should not simply mean:

> "New to our organisation."

Something may be new internally while already being a mature commodity externally.

---

# Stage 2 – Custom Built

As understanding increases, useful solutions begin to emerge.

Characteristics may include:

```text
Bespoke

Specialist

Increasing understanding

Emerging practices

Limited suppliers

High variation

Designed for specific needs
```

Organisations may still require significant specialist capability at this stage.

---

# Stage 3 – Product

The component becomes increasingly understood and supplied as a repeatable product or service.

Characteristics may include:

```text
Established market

Multiple suppliers

Feature competition

Increasing standardisation

Known practices

Improved reliability

More predictable delivery
```

Differentiation may still exist, but the component is no longer genuinely novel.

---

# Stage 4 – Commodity / Utility

The component becomes highly industrialised.

Characteristics may include:

```text
Standard

Widely available

Highly understood

Volume focused

Efficiency focused

Low differentiation

Utility consumption where appropriate
```

Examples frequently include infrastructure services or other capabilities where the organisation gains limited strategic differentiation from recreating the underlying component itself.

---

# Evolution is Not a Technology Lifecycle

Evolution should not simply be interpreted as:

```text
Old
        →
New
```

A newly released product may already represent a highly evolved component.

Similarly, an old organisational capability might remain poorly understood or highly bespoke.

The question is not:

> How old is it?

The question is:

> What are the characteristics of the component and its surrounding market?

---

# Start With the User

Wardley Mapping begins with the user and their need.

Wardley's doctrine explicitly emphasises focusing on user need as the anchor for a map (Wardley, 2016–2018).

Possible users might include:

```text
Customer

Viewer

Advertiser

Distributor

Finance Director

Sales Executive

Marketing Manager

Analyst

Regulator

Employee
```

The user does not have to be an external customer.

For an internal Data Product, the user might be:

```text
Finance Director
```

with the need:

```text
Understand current and forecast financial performance.
```

---

# User Need

The next question is:

> **What does the user actually need?**

Avoid confusing user needs with organisational needs.

For example:

```text
BUSINESS NEED

Increase Revenue
```

may not represent the customer's need.

A customer need might instead be:

```text
Find suitable content quickly.
```

By meeting that customer need effectively, the organisation may subsequently achieve its own commercial objective.

The distinction is important.

---

# Discovering the Value Chain

Once the user need is understood, identify what is required to satisfy it.

Ask repeatedly:

> **What does this depend upon?**

For example:

```text
Finance Director

        │
        ▼

Understand Financial Performance

        │
        ▼

Financial Analytics

        │
        ▼

Governed Financial Measures

        │
        ▼

Finance Data Product

        │
        ▼

Finance Source Data

        │
        ▼

Operational Systems
```

This dependency chain provides the starting structure for the map.

---

# Dependencies

Relationships in a Wardley Map describe dependency.

For example:

```text
Management Reporting
        │
        ▼
Revenue KPI
        │
        ▼
Revenue Data
        │
        ▼
Contract Data
```

This indicates:

```text
Management Reporting

NEEDS

Revenue KPI

WHICH NEEDS

Revenue Data

WHICH NEEDS

Contract Data
```

The map therefore provides useful visibility of dependencies that may otherwise be hidden.

---

# Mapping Components

Potential map components may include:

- User Needs
- Business Capabilities
- Activities
- Practices
- Data
- Data Products
- Technology
- Platforms
- Services
- External Providers

Do not put everything in the organisation onto one map.

The components should support the strategic question being explored.

---

# Start Small

A useful first Wardley Map may contain only:

```text
One User

One Primary Need

5–15 Important Components
```

The objective is not to create an exhaustive inventory.

The objective is to improve understanding of the landscape.

The map can be expanded as discovery progresses.

---

# Positioning Components

Once the chain of needs has been identified, position each component against the evolution axis.

Ask:

```text
How novel is this?

How well understood is it?

Is there an established market?

Are there multiple suppliers?

Are standards established?

Is best practice known?

Does this genuinely differentiate us?

Could we readily obtain this externally?

Would customers value us building this ourselves?
```

The discussion about positioning can be more valuable than achieving a supposedly perfect position.

---

# Position is a Hypothesis

Wardley Maps should not be treated as objective measurements of reality.

The initial position of a component represents a hypothesis.

For example:

```text
Participant A

"This is Custom Built."


Participant B

"No — there are dozens of mature products available."
```

This disagreement is useful.

It may expose:

- Lack of market awareness
- Organisational bias
- Different definitions
- Legacy thinking
- Strategic assumptions

Capture and investigate the disagreement.

---

# Movement

An important characteristic of a Wardley Map is that components can evolve.

For example:

```text
Custom Built Analytics Platform

              ───────────────►

Commercial Analytics Product

              ───────────────►

Commodity Analytics Capability
```

This allows strategic discovery to ask:

```text
Where is this component likely to move?

What happens when it moves?

What becomes possible?

Which existing investments become less valuable?

Where will new opportunities emerge?
```

Wardley Mapping therefore introduces a temporal and evolutionary perspective that many static business diagrams lack.

---

# Componentisation

As lower-level components become increasingly industrialised, higher-level components can often be created more easily.

Conceptually:

```text
Industrialised Component
           │
           ▼
Lower Cost / Easier Consumption
           │
           ▼
Enables New Higher-Order Components
           │
           ▼
New Innovation
```

For example, commodity cloud infrastructure enabled organisations to build digital capabilities without first constructing physical computing infrastructure.

Wardley uses this relationship between industrialisation and higher-order innovation extensively within the wider mapping framework (Wardley, 2016–2018).

---

# Inertia

Evolution does not mean organisations automatically change with the market.

Existing success, investment, skills, practices and operating models can create **inertia**.

For example:

```text
Component Evolves

Custom Built
      │
      ▼
Commodity
```

while the organisation continues operating it as:

```text
Custom Built
```

Possible reasons include:

- Existing investment
- Organisational structure
- Specialist roles
- Supplier contracts
- Legacy processes
- Existing business models
- Cultural attachment
- Fear of change

Wardley identifies inertia associated with past success as an important pattern affecting organisational response to evolution (Wardley, 2016–2018).

---

# Strategic Misalignment

One of the most useful DISCOVER applications of Wardley Mapping is identifying where the organisation's approach does not fit the evolutionary position of a component.

For example:

```text
COMPONENT

Commodity Infrastructure


CURRENT APPROACH

Custom Building Everything Internally
```

This should trigger the question:

> **Why?**

There may be a legitimate reason.

For example:

```text
Security

Regulation

Extreme Performance

Unique Constraint
```

But there should be evidence.

Otherwise, the organisation may be investing effort in an area that provides little differentiation.

---

# One Size Does Not Fit All

Different evolutionary stages can require different approaches.

Conceptually:

```text
Genesis

Experiment
Explore
Learn
Accept uncertainty


Custom Built

Develop
Refine
Understand
Build capability


Product

Manage
Optimise
Compete
Standardise


Commodity

Industrialise
Automate
Measure
Focus on efficiency
```

Wardley argues against applying the same methods uniformly across the entire landscape because components at different stages exhibit different characteristics (Wardley, 2016–2018).

DISCOVER uses this principle cautiously.

The map should help provoke questions about the most appropriate approach rather than mechanically prescribe one delivery methodology.

---

# Build, Buy or Consume

Wardley Mapping can provide valuable context for sourcing decisions.

A simplified heuristic might be:

```text
Genesis
   │
   └── Explore / Experiment

Custom Built
   │
   └── Build where differentiation matters

Product
   │
   └── Consider market products

Commodity
   │
   └── Consume standardised services where appropriate
```

This is not an automatic decision rule.

Additional considerations include:

- Strategic differentiation
- Regulation
- Security
- Cost
- Capability
- Vendor risk
- Data sovereignty
- Integration
- Switching cost

The map provides context for the decision rather than replacing analysis.

---

# Duplication

Wardley Maps created across several business areas can expose duplication.

For example:

```text
Finance Map
    └── Custom Reporting Platform

Marketing Map
    └── Custom Reporting Platform

Sales Map
    └── Custom Reporting Platform
```

Further investigation may reveal that each team has independently created similar commodity capabilities.

Potential response:

```text
Shared Analytics Capability
```

or:

```text
Common Data Platform
```

However, apparent duplication should be validated.

Two components with similar names may serve different needs.

---

# Strategy Before Technology

Wardley Mapping reinforces a useful DISCOVER principle:

> **Technology choices should be informed by business context.**

Avoid beginning with:

```text
We need a Knowledge Graph.

We need GenAI.

We need a Data Mesh.

We need a new CRM.

We need a Lakehouse.
```

Instead begin with:

```text
Who is the user?

What do they need?

What capabilities are required?

What do those capabilities depend upon?

How evolved are those components?

Where does differentiation matter?
```

Only then evaluate technology.

---

# Wardley Mapping Workshop

A DISCOVER Wardley Mapping workshop might follow this structure.

| Stage | Activity |
|-------|----------|
| 1 | Define strategic question |
| 2 | Identify user |
| 3 | Identify user needs |
| 4 | Identify major components |
| 5 | Identify dependencies |
| 6 | Build value chain |
| 7 | Position components by evolution |
| 8 | Challenge assumptions |
| 9 | Identify movement |
| 10 | Identify inertia |
| 11 | Identify duplication |
| 12 | Explore strategic options |
| 13 | Capture opportunities |
| 14 | Agree further investigation |

The workshop should be exploratory.

Do not spend excessive time arguing about the exact horizontal position of every component.

---

# Define the Strategic Question

Every map should have a purpose.

Examples:

```text
Where should we invest in our Data & Analytics capability?

Which Finance capabilities should we build versus buy?

Where could AI create strategic advantage?

How should our content data platform evolve?

Where are we recreating commodity capabilities?

Which parts of this business capability genuinely differentiate us?
```

Without a clear question, a map can become an interesting picture with no strategic purpose.

---

# Generic Discovery Questions

## User

- Who is the user?
- Are there several types of user?
- What outcome are they trying to achieve?
- What do they genuinely need?
- How do we know?

---

## Value Chain

- What is required to meet that need?
- What does each component depend upon?
- What enables the component above it?
- Are any dependencies missing?
- Which dependencies exist outside the organisation?

---

## Evolution

- How novel is this component?
- Is it well understood?
- Is an established market available?
- Are there multiple suppliers?
- Are standard practices established?
- Is it truly unique?

---

## Differentiation

- Does this component differentiate us?
- Does the user care how this component is provided?
- What competitive advantage comes from owning it?
- Are we investing heavily in something customers consider standard?

---

## Movement

- How is this component likely to evolve?
- What is causing that movement?
- What happens when it becomes more industrialised?
- What new capabilities could that enable?
- Which existing investments might become obsolete?

---

## Inertia

- What prevents us from changing?
- Which existing investments depend upon the current model?
- Which roles or teams are affected?
- Which existing processes assume the current approach?
- What would become redundant if the component evolved?

---

## Sourcing

- Should we build this?
- Could we buy it?
- Could we consume it as a service?
- Why are we building something that already exists?
- Where does internal development create genuine strategic value?

---

## Duplication

- Does another team have the same capability?
- Are several systems solving the same problem?
- Could this become a shared component?
- Why does each area need its own implementation?

---

## Investment

- Where should investment increase?
- Where should investment decrease?
- Which components require experimentation?
- Which components require industrialisation?
- Which capabilities deserve differentiation?

---

# Mapping Existing Technology

Technology can be added after user needs and dependencies are understood.

For example:

```text
User Need
   │
   ▼
Financial Insight
   │
   ▼
Analytics
   │
   ▼
Finance Data Product
   │
   ▼
Data Platform
   │
   ▼
Cloud Infrastructure
```

The resulting map may reveal:

```text
Financial Insight     → Differentiating

Finance Data Product  → Organisation-specific

Data Platform         → Product / increasingly standardised

Cloud Infrastructure  → Utility
```

This can focus investment more intelligently.

The organisation may wish to differentiate through:

```text
Financial Insight
```

rather than through:

```text
Building its own compute infrastructure.
```

---

# Wardley Mapping and Business Capability Mapping

Capability Mapping asks:

> **What must the organisation be able to do?**

Wardley Mapping adds:

> **What does that capability depend upon, and how evolved are those components?**

For example:

```text
CAPABILITY MAP

Revenue Management
        │
        ├── Forecasting
        ├── Revenue Recognition
        └── Reporting
```

Wardley Mapping might then explore:

```text
Finance Director
      │
      ▼
Financial Performance Insight
      │
      ▼
Revenue Analytics
      │
      ▼
Revenue Data Product
      │
      ▼
Finance Data Platform
      │
      ▼
Cloud Infrastructure

Genesis  Custom  Product  Commodity
```

The two techniques therefore provide complementary perspectives.

---

# Wardley Mapping and Value Stream Mapping

Despite the word "value", Wardley Mapping and Value Stream Mapping are different techniques.

Value Stream Mapping asks:

> **How does value flow from need to outcome?**

Wardley Mapping asks:

> **What components make that outcome possible and how are those components evolving?**

Conceptually:

```text
VALUE STREAM MAPPING

Customer Need
     │
     ▼
Activities
     │
     ▼
Flow
     │
     ▼
Customer Outcome
```

versus:

```text
WARDLEY MAPPING

User Need
     │
     ▼
Dependencies
     │
     ▼
Components
     │
     +
Evolution
```

A useful DISCOVER pattern is to use both where appropriate.

---

# Wardley Mapping and Process Modelling

Process Modelling explains:

```text
How Work Happens
```

Wardley Mapping examines:

```text
The Strategic Landscape
```

For example:

```text
PROCESS FINDING

Analyst manually reconciles
three spreadsheets.
```

Wardley Mapping may ask:

```text
Why are we custom building
a capability that has become
standardised elsewhere?
```

The techniques therefore operate at different levels of analysis.

---

# Wardley Mapping and POPIT-V

Wardley Mapping can enrich every POPIT-V perspective.

## People

- Do we have skills appropriate to the component's evolutionary stage?
- Is specialist knowledge concentrated around legacy components?
- Where could changing technology affect roles?

## Organisation

- Which capabilities differentiate us?
- Where does ownership sit?
- Is organisational structure creating inertia?

## Process

- Do our methods suit the nature of the component?
- Are mature activities still being managed experimentally?
- Are emerging activities constrained by excessive governance?

## Information

- Which information assets are strategically differentiating?
- Which information is commonly available?
- Which data products enable higher-order capabilities?

## Technology

- Where are we custom building commodity technology?
- Which components should be products or utilities?
- Where is legacy technology constraining movement?

## Value

- What does the user actually need?
- Which components contribute most strongly to that need?
- Where will investment create strategic advantage?

---

# Wardley Mapping and Data Strategy

Wardley Mapping can be particularly useful when creating a Data & Analytics strategy.

Consider a simplified landscape:

```text
                         Decision Maker
                               │
                               ▼
                         Business Insight
                               │
                    ┌──────────┴──────────┐
                    ▼                     ▼
              Predictive Model       Analytics
                    │                     │
                    └──────────┬──────────┘
                               ▼
                          Data Product
                               │
                               ▼
                       Semantic / Data Layer
                               │
                               ▼
                         Data Platform
                               │
                               ▼
                     Cloud Infrastructure
```

The map might suggest:

```text
Business Insight
        →
Strategic / Context Specific


Predictive Models
        →
Potential Differentiation


Domain Data Products
        →
Business Specific


Generic Data Processing
        →
Increasingly Productised


Cloud Infrastructure
        →
Utility
```

This helps answer:

> **Where should scarce organisational capability be concentrated?**

The answer may be closer to business knowledge, domain data and decision-making than underlying infrastructure.

---

# Wardley Mapping and Data Products

Data Products can themselves be placed on a Wardley Map.

For example:

```text
Finance Director
       │
       ▼
Financial Insight
       │
       ▼
Revenue Performance
Data Product
       │
       ▼
Finance Semantic Layer
       │
       ▼
Data Platform
       │
       ▼
Cloud Infrastructure
```

Useful questions include:

- Is this Data Product truly unique?
- Which domain knowledge makes it valuable?
- Which underlying capabilities can be standardised?
- Which dependencies are commodity services?
- Where should Product ownership sit?
- What happens as underlying technology evolves?

This can prevent Data Product teams from spending excessive effort recreating lower-level commodity capabilities.

---

# Wardley Mapping and AI

Wardley Mapping can provide valuable strategic context for AI discovery.

An organisation may initially state:

```text
"We need AI."
```

A Wardley Map forces deeper questions.

For example:

```text
User
  │
  ▼
Decision
  │
  ▼
Business Knowledge
  │
  ▼
AI Capability
  │
  ▼
Model
  │
  ▼
Compute
```

These components may sit in very different evolutionary positions.

For example:

```text
Business-Specific Decision Context
        →
Highly differentiated


Domain Knowledge
        →
Organisation specific


Generic Foundation Model
        →
Increasingly productised


Compute
        →
Utility
```

This may suggest that competitive advantage lies less in building a general-purpose foundation model and more in combining increasingly standardised AI capabilities with:

```text
Proprietary Data

Domain Knowledge

Business Rules

Ontology

Workflow

User Experience
```

The map should inform the AI strategy rather than automatically determine it.

---

# Example – AI Knowledge Assistant

Consider:

```text
Employee
   │
   ▼
Find Trusted Business Answer
   │
   ▼
Knowledge Assistant
   │
   ├───────────┐
   ▼           ▼
Domain      Enterprise
Ontology    Search
   │           │
   └─────┬─────┘
         ▼
   Business Content
         │
         ▼
     LLM Service
         │
         ▼
       Compute
```

The map may expose that:

```text
LLM Service
        →
Increasingly standardised


Compute
        →
Commodity / Utility


Business Content
        →
Organisation specific


Domain Ontology
        →
Potential strategic capability


Trusted Answer Experience
        →
Potential differentiation
```

This reframes the question from:

> Which LLM should we build?

to:

> Which parts of the complete capability genuinely create differentiated business value?

---

# Finance Example

## Discovery Objective

Understand where Finance technology and Data & Analytics investment should be concentrated.

An initial map could identify:

```text
                         CFO
                          │
                          ▼
                  Understand Financial
                     Performance
                          │
              ┌───────────┴───────────┐
              ▼                       ▼
        Financial Forecast       Management
                                Reporting
              │                       │
              └───────────┬───────────┘
                          ▼
                  Finance Data Product
                          │
               ┌──────────┴──────────┐
               ▼                     ▼
          Contract Data        Financial Actuals
               │                     │
               └──────────┬──────────┘
                          ▼
                     Data Platform
                          │
                          ▼
                  Cloud Infrastructure
```

### Discovery Questions

- What does the CFO need to understand?
- Which information directly supports financial decisions?
- Which Finance capabilities differentiate the organisation?
- Which capabilities are regulatory necessities?
- Where are bespoke spreadsheets recreating common functionality?
- Which Finance technology is now commoditised?
- Which specialist business rules genuinely need internal ownership?
- What would happen if commodity components were replaced?
- Where does Finance have inertia?
- Which capabilities should become shared Data Products?

### Potential Findings

Discovery may reveal:

```text
Cloud infrastructure is already consumed as a utility.

Data integration is increasingly standardised.

Financial data models remain organisation specific.

Revenue recognition contains specialist domain knowledge.

Forecast models may create competitive value.

Multiple teams independently build similar reporting capabilities.

Legacy spreadsheets create inertia.
```

### Potential Strategic Direction

The resulting direction might be:

```text
BUY / CONSUME

Infrastructure
Generic Processing
Commodity Tooling


STANDARDISE

Finance Semantic Layer
Common KPIs
Shared Reference Data


OWN / DIFFERENTIATE

Revenue Logic
Commercial Knowledge
Forecasting
Decision Support
```

This should remain a hypothesis until validated through wider discovery.

### Potential Opportunities

- Finance Data Product
- Revenue Semantic Layer
- Revenue Rules Catalogue
- Shared Finance Analytics Capability
- Forecasting Product
- Finance Knowledge Assistant
- Rationalisation of Duplicate Reporting Platforms

---

# Marketing Example

## Discovery Objective

Understand where Marketing should differentiate and where it should consume standard market capabilities.

An initial map might include:

```text
                     Marketing Manager
                            │
                            ▼
                  Improve Campaign
                     Performance
                            │
                ┌───────────┴───────────┐
                ▼                       ▼
          Audience Insight        Campaign Insight
                │                       │
                └───────────┬───────────┘
                            ▼
                  Marketing Data Product
                            │
              ┌─────────────┼─────────────┐
              ▼             ▼             ▼
          Audience       Campaign       Spend
           Data            Data         Data
              │             │             │
              └─────────────┼─────────────┘
                            ▼
                    Marketing Platforms
                            │
                            ▼
                    Cloud Infrastructure
```

### Discovery Questions

- What genuinely differentiates Marketing performance?
- Is campaign execution technology a source of differentiation?
- Is audience knowledge more valuable than the underlying platform?
- Which capabilities are standard across the market?
- Are multiple teams building similar integrations?
- Where is proprietary first-party data important?
- Where could prediction create competitive advantage?
- Which marketing capabilities are likely to become more commoditised?

### Potential Findings

Discovery may reveal:

```text
Campaign execution platforms are highly productised.

Infrastructure provides little differentiation.

Audience understanding remains organisation specific.

Historical campaign performance is poorly exploited.

Campaign optimisation could provide differentiation.

Platform integrations are duplicated across teams.
```

### Potential Strategic Direction

```text
CONSUME

Advertising Platforms
Cloud Infrastructure
Generic AI Models


STANDARDISE

Campaign Metadata
Campaign Taxonomy
Integration Patterns
Performance KPIs


DIFFERENTIATE

Audience Intelligence
Campaign Optimisation
Customer Knowledge
Predictive Performance
```

### Potential Opportunities

- Audience Data Product
- Campaign Performance Data Product
- Marketing Ontology
- Predictive Campaign Optimisation
- Shared Marketing Integration Layer
- AI Campaign Insight Assistant

---

# Mapping an Enterprise Data Platform

Wardley Mapping can help challenge a common assumption:

```text
"The Data Platform is the product."
```

Consider:

```text
Business User
      │
      ▼
Business Decision
      │
      ▼
Insight
      │
      ▼
Data Product
      │
      ▼
Semantic Layer
      │
      ▼
Data Platform
      │
      ▼
Cloud
```

The closer the component is to:

```text
Business Decision
```

the more likely business context matters.

The lower infrastructure components may increasingly be standardised.

This can help ensure platform investment remains connected to user needs rather than becoming an objective in itself.

---

# Mapping Ontology and Semantic Capabilities

Ontology can also be positioned strategically.

For example:

```text
Business User
      │
      ▼
Business Question
      │
      ▼
Semantic Understanding
      │
      ▼
Enterprise Ontology
      │
      ├────────────► Business Glossary
      │
      ├────────────► Data Products
      │
      └────────────► Knowledge Graph
                           │
                           ▼
                       Technology
```

The technology used to store an ontology may be increasingly standardised.

The organisation's own:

```text
Business Concepts

Relationships

Rules

Terminology

Knowledge
```

may remain highly context specific.

This distinction can help organisations invest in business knowledge rather than unnecessarily differentiating through technical implementation.

---

# Strategic Patterns

The wider Wardley Mapping framework includes a range of recurring patterns, doctrines and forms of gameplay.

DISCOVER does not attempt to reproduce the full framework.

However, several ideas are particularly useful during discovery:

```text
Focus on User Needs

Understand the Landscape

Challenge Assumptions

Remove Unnecessary Duplication

Use Appropriate Methods

Think Small

Consider Evolution

Expect Inertia

Design for Change
```

Wardley describes these types of broadly applicable operating principles as **doctrine** (Wardley, 2016–2018).

Practitioners wishing to use Wardley Mapping for detailed competitive strategy should consult Wardley's original material.

---

# Pioneers, Settlers and Town Planners

Wardley's wider framework also describes different attitudes suited to different stages of evolution.

Conceptually:

```text
PIONEERS

Explore the novel
Experiment
Operate with uncertainty


SETTLERS

Turn emerging ideas into useful,
repeatable products


TOWN PLANNERS

Industrialise established components
for scale, reliability and efficiency
```

The idea is that different types of work may benefit from different organisational behaviours rather than forcing a single culture or operating method across everything (Wardley, 2016–2018).

Within DISCOVER, this concept can be useful when analysing:

- Team design
- Product ownership
- Innovation
- Platform development
- Data Product maturity
- AI experimentation

It should be used as a discussion aid rather than a rigid classification of individuals.

---

# Wardley Mapping and Roadmaps

A Wardley Map is **not a roadmap**.

A roadmap usually describes intended activity over time:

```text
Q1
   │
   ▼
Build Capability

Q2
   │
   ▼
Launch Product

Q3
   │
   ▼
Expand
```

A Wardley Map describes the current strategic landscape and possible movement.

Conceptually:

```text
WARDLEY MAP

Where are we?

What is changing?

What options exist?

        │
        ▼

ROADMAP

Given that understanding,
what will we do and when?
```

Within DISCOVER, Wardley Mapping can therefore provide an input into Roadmapping.

---

# Wardley Mapping and Prioritisation

A map can expose opportunities such as:

```text
Invest

Standardise

Industrialise

Experiment

Consolidate

Buy

Consume

Retire
```

These should not automatically enter the roadmap.

They should feed into the DISCOVER Opportunity Register and Prioritisation process.

Assessment can then consider:

- Business Value
- Strategic Alignment
- User Impact
- Effort
- Risk
- Dependencies
- Data Readiness
- Technology Readiness

This maintains separation between:

```text
Strategic Discovery
        │
        ▼
Opportunity
        │
        ▼
Evaluation
        │
        ▼
Prioritisation
        │
        ▼
Roadmap
```

---

# Mapping Competitors

Wardley Maps may also be used to explore competitors or alternative strategic positions.

For example:

```text
Our Position

Custom Built Component
```

versus:

```text
Competitor

Consumes Commodity Service
```

This may lead to:

```text
Competitor has lower operating cost

Competitor can invest more heavily
in higher-order differentiation
```

However, competitor positions are often based upon incomplete information.

Clearly identify assumptions and uncertainty.

---

# Mapping External Change

Wardley Mapping can also support strategic discussion around market evolution.

Ask:

```text
Which components are moving?

Which products are becoming utilities?

Which previously scarce capabilities are becoming widely available?

What will this enable?

What existing business models depend upon scarcity?

Where might inertia prevent us from responding?
```

This can help identify emerging threats and opportunities.

---

# Mapping Uncertainty

Not every component can be positioned confidently.

Use annotations where necessary:

```text
High Confidence

Medium Confidence

Low Confidence

Requires Research
```

This transforms uncertainty into an explicit discovery action.

For example:

```text
AI Metadata Extraction

Evolution = ?

ACTION

Market Assessment
```

The map therefore helps identify what the team does not yet know.

---

# Evidence

Where important strategic decisions depend upon map position, gather evidence.

Possible evidence includes:

- Market Research
- Supplier Analysis
- Cost Analysis
- Technology Assessment
- User Research
- Capability Assessment
- Vendor Landscape
- Internal Usage
- Industry Standards

Wardley Mapping should improve strategic reasoning.

It should not simply replace unsupported opinion with dots on a diagram.

---

# Connecting Wardley Mapping to the DISCOVER Golden Thread

Wardley Mapping can provide strategic context across the DISCOVER Golden Thread.

```text
Business Strategy
        │
        ▼
Business Capability
        │
        ▼
User Need
        │
        ▼
Business Decision
        │
        ▼
Business Information
        │
        ▼
Data Product
        │
        ▼
Technology
        │
        ▼
Evolution
        │
        ▼
Strategic Choice
        │
        ▼
Roadmap
        │
        ▼
Business Value
```

This makes Wardley Mapping especially useful when discovery moves from understanding the organisation towards deciding **where to invest**.

---

# Common Pitfalls

## Starting With Technology

Avoid beginning with:

```text
Where should Databricks sit?

Where should Salesforce sit?

Where should Vertex AI sit?
```

Start with:

```text
Who is the user?

What do they need?
```

Then discover the components required.

---

## Creating an Architecture Diagram

A Wardley Map is not simply another technology architecture diagram.

Evolution and user dependency are essential.

Without them it is not providing the strategic perspective that makes Wardley Mapping distinctive.

---

## Confusing Evolution With Maturity

A component can be:

```text
Well Managed

but

Custom Built
```

or:

```text
Poorly Managed

but

Commodity
```

Evolution and organisational maturity are different concepts.

---

## Assuming New Means Genesis

A technology introduced last month may already be highly productised.

Assess the external landscape, not simply internal adoption.

---

## Treating Placement as Fact

Map positions are hypotheses.

Challenge them.

---

## Mapping Everything

An unreadable map creates little strategic insight.

Focus on components relevant to the strategic question.

---

## Using Evolution as an Automatic Sourcing Rule

Do not blindly apply:

```text
Commodity = Outsource
```

Real decisions must consider context, risk and value.

---

## Ignoring User Need

Without a user and need, the map loses its anchor.

---

## Ignoring Movement

A static map provides less value.

Ask how important components are changing.

---

## Ignoring Inertia

Knowing that something should change does not mean the organisation can change easily.

Understand the constraints.

---

## Mapping Without Decision

A Wardley Map should support strategic thinking.

If the map does not influence:

```text
Investment

Prioritisation

Architecture

Sourcing

Product Strategy

Roadmap
```

ask why it is being created.

---

# What Good Looks Like

An effective Wardley Map should:

- Have a clear strategic question
- Identify the relevant user
- Define meaningful user needs
- Show important components
- Show dependencies
- Position components by evolution
- Make assumptions visible
- Identify likely movement
- Expose possible inertia
- Highlight duplication
- Reveal strategic choices
- Generate useful discussion
- Be understandable by participants
- Support subsequent prioritisation and roadmapping

The objective is not to create the perfect map.

The objective is to improve **situational awareness**.

---

# Discovery Outputs

Wardley Mapping should contribute to:

- Wardley Map
- User Needs
- Dependency Model
- Strategic Landscape
- Evolution Assessment
- Inertia Assessment
- Duplication Findings
- Build / Buy / Consume Analysis
- Strategic Opportunities
- Technology Strategy
- Data Strategy
- AI Strategy
- Opportunity Register
- Prioritisation
- Roadmap

---

# Related DISCOVER Techniques

Wardley Mapping works particularly well alongside:

- Business Capability Mapping
- Stakeholder Mapping
- Value Stream Mapping
- Process Modelling
- Domain-Driven Design
- Ontology Discovery
- Data Product Design
- AI Opportunity Discovery
- Prioritisation
- Roadmapping

A possible progression is:

```text
Business Strategy
       │
       ▼
Business Capability Mapping
       │
       ▼
User / Stakeholder Discovery
       │
       ▼
Wardley Mapping
       │
       ├────────────► User Needs
       ├────────────► Dependencies
       ├────────────► Evolution
       ├────────────► Inertia
       └────────────► Strategic Options
                           │
                           ▼
                      Opportunities
                           │
                           ▼
                      Prioritisation
                           │
                           ▼
                        Roadmap
```

The sequence is illustrative rather than mandatory.

---

# Recommended Discovery Questions – Quick Reference

Before concluding a Wardley Mapping exercise, ensure you can answer:

- What strategic question are we exploring?
- Who is the user?
- What does that user need?
- What components are required to satisfy that need?
- What does each component depend upon?
- Which components are genuinely novel?
- Which are bespoke?
- Which are established products?
- Which are commodities or utilities?
- How confident are we in those positions?
- Which components genuinely differentiate the organisation?
- Where are we custom building commodity capabilities?
- Where is there duplication?
- Which components are likely to evolve?
- What will their evolution enable?
- Where does organisational inertia exist?
- Which capabilities should we experiment with?
- Which should we standardise?
- Which should we industrialise?
- Which should we buy or consume?
- Where should investment increase?
- Where should investment decrease?
- Which Data Products create strategic value?
- Where does proprietary business knowledge matter?
- Where could AI create differentiation?
- Which AI capabilities are becoming commodity services?
- What opportunities should move into prioritisation?
- What requires further investigation?

---

# References

Cringely, R.X. (1993) *Accidental Empires: How the Boys of Silicon Valley Make Their Millions, Battle Foreign Competition, and Still Can't Get a Date*. Reading, MA: Addison-Wesley.

Learn Wardley Mapping (n.d.) *Introduction*. Available at: https://learnwardleymapping.com/introduction/ (Accessed: 10 August 2026).

Learn Wardley Mapping (n.d.) *Landscape*. Available at: https://learnwardleymapping.com/landscape/ (Accessed: 10 August 2026).

Wardley, S. (2016–2018) *Wardley Maps: Topographical Intelligence in Business*. Available at: https://www.swardleymaps.com/writings-books (Accessed: 10 August 2026).

Wardley, S. (2016) 'On Being Lost', *Wardley Maps*, Medium. Available at: https://medium.com/wardleymaps/on-being-lost-2ef5f05eb1ec (Accessed: 10 August 2026).

Wardley, S. (2016) 'Doctrine', *Wardley Maps*, Medium. Available at: https://medium.com/wardleymaps/doctrine-8bb0015688e5 (Accessed: 10 August 2026).

Wardley, S. (2016) 'Getting Started', *Wardley Maps*, Medium. Available at: https://medium.com/wardleymaps/getting-started-yourself-e1a359b785a2 (Accessed: 10 August 2026).