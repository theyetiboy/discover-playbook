# Data Source / Data Asset Catalogue

> Map physical data to business meaning. A data catalogue should not replace the business glossary or ontology.

## Context

| Field | Value |
|---|---|
| Domain | |
| Discovery Objective | |
| Prepared By | |
| Date | |
| Status | |

## Data Asset Catalogue

| Data Asset ID | Asset / Dataset | Source System | Business Purpose | Business Concepts Represented | Grain | Owner | Steward / Custodian | Refresh / Latency | Sensitivity | Quality Expectations | Lineage Available? | Consumers | Evidence | Status |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| `DAT-001` | | `SYS-001` | | `INF-001` | | | | | | | Yes / No / Partial | | `EVD-001` | Unvalidated |

## Source System Catalogue

| System ID | System | Business Purpose | Capability Supported | System Owner | Vendor / Platform | Criticality | Lifecycle | Notes |
|---|---|---|---|---|---|---|---|---|
| `SYS-001` | | `CAP-001` | | | | | Live / Legacy / Planned | |

## Physical Mapping

Use this when connecting semantic concepts to source data.

| Information / Concept ID | Business Concept | Data Asset ID | Physical Object / Field | Transformation / Mapping | Authoritative for Which Context? | Evidence | Status |
|---|---|---|---|---|---|---|---|
| `INF-001` | | `DAT-001` | | | | | |

## Data Quality Requirements

Quality should be defined in relation to a decision/use case.

| Data Asset ID | Decision / Use Case | Quality Dimension | Requirement / Threshold | Current Evidence | Business Impact if Breached | Owner | Status |
|---|---|---|---|---|---|---|---|
| `DAT-001` | `DEC-001` | Accuracy / Completeness / Timeliness / Consistency / Validity / Uniqueness / Integrity | | | | | |

## Freshness and Availability

| Data Asset ID | Required Freshness | Current Freshness | Availability / SLA | Consumer Need | Gap / Impact |
|---|---|---|---|---|---|
| | | | | | |

## Lineage / Provenance

| Data Asset ID | Upstream Source | Transformation / Rule | Downstream Asset / Report | Manual Adjustment? | Provenance Evidence | Known Gap |
|---|---|---|---|---|---|---|
| | | | | | | |

## Data Access / Governance

| Data Asset ID | Classification | Personal / Sensitive Data | Access Model | Retention | Regulatory / Contractual Constraints | Owner |
|---|---|---|---|---|---|---|
| | | | | | | |

## Pain Points

| Pain ID | Data Asset ID | Problem | Decision / Process Impact | Evidence | Root Cause Established? | Validation Needed |
|---|---|---|---|---|---|---|
| `PAIN-001` | | | | | Yes / No | |

## Data Product Readiness Questions

Before treating an asset as a data product ask:

- Who is the consumer?
- Which decision/action does it support?
- What business concepts does it expose?
- What ownership and service expectations exist?
- What quality/freshness is required?
- What documentation/metadata is needed?
- What measurable value is expected?

## Checklist

- [ ] Business concepts mapped separately from physical schema.
- [ ] Owners and custodians distinguished.
- [ ] Grain and freshness understood.
- [ ] Quality requirements tied to use.
- [ ] Sensitivity/access captured.
- [ ] Lineage/provenance known or gaps explicit.
- [ ] Manual adjustments visible.
- [ ] Authoritative-source claims are contextual.
- [ ] Candidate data products are not inferred solely from datasets.
