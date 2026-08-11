# Ontology Discovery Capture

> Capture business concepts and relationships before choosing a formal semantic implementation.

## Context

| Field | Value |
|---|---|
| Domain / Bounded Context | |
| Discovery Objective | |
| Business Questions / Decisions | |
| Prepared By | |
| Date | |
| Semantic Owner | |
| Status | |

## Competency Questions

Start here. What should the semantic model help people or systems answer?

| CQ ID | Competency Question | User / Decision | Priority | Evidence / Source | Status |
|---|---|---|---|---|---|
| `CQ-001` | | `DEC-001` | High / Medium / Low | | |

## Concept Catalogue

| Concept ID | Preferred Concept | Definition | Context | Concept Type | Synonyms | Owner | Evidence | Validation Status |
|---|---|---|---|---|---|---|---|---|
| `INF-001` | | | | Class / Concept / Vocabulary | | | `EVD-001` | Unvalidated |

## Instance Examples

Use examples to validate meaning; do not confuse instances with concepts.

| Concept ID | Example Instance | Why Useful | Evidence |
|---|---|---|---|
| | | | |

## Relationship Catalogue

| Relationship ID | Subject Concept | Relationship / Predicate | Object Concept | Definition | Cardinality / Constraint | Context / Temporal Rule | Evidence | Status |
|---|---|---|---|---|---|---|---|---|
| `REL-001` | `INF-001` | grants / owns / part of / applies in / etc. | `INF-002` | | UNKNOWN until validated | | | |

## Hierarchies / Taxonomies

| Parent Concept | Child Concept | Relationship Type | Context | Evidence | Status |
|---|---|---|---|---|---|
| | | is-a / broader-narrower / part-of | | | |

## Business Rules / Constraints

| Rule ID | Rule | Related Concepts / Relationships | Owner | Evidence | Status |
|---|---|---|---|---|---|
| `BR-001` | | | | | |

## Context / Bounded Context Differences

| Term / Concept | Context A Meaning | Context B Meaning | Translation / Relationship | Owners | Validation Needed |
|---|---|---|---|---|---|
| | | | | | |

## Identity / Identifier Mapping

| Concept ID | Business Identity | System | Physical Identifier | Cross-reference Available? | Known Issue |
|---|---|---|---|---|---|
| | | `SYS-001` | | | |

## Source-to-Concept Mapping

| Concept ID | Data Asset ID | Physical Object / Field | Mapping Rule | Provenance | Status |
|---|---|---|---|---|---|
| `INF-001` | `DAT-001` | | | | Candidate |

## Competency Question Coverage

| CQ ID | Required Concepts | Required Relationships / Rules | Data Mapping Available? | Gap / Broken Thread |
|---|---|---|---|---|
| `CQ-001` | | | | |

## Potential Formal Representation

Only complete if implementation is justified.

| Need | Candidate Standard / Pattern | Rationale | Decision Status |
|---|---|---|---|
| Graph statements | RDF | | |
| Ontology semantics | OWL 2 | | |
| Controlled vocabulary | SKOS | | |
| Graph constraints | SHACL | | |
| Provenance | PROV-O | | |
| Catalogue semantics | DCAT 3 | | |

## Governance

| Governance Area | Owner | Process | Evidence / Standard | Status |
|---|---|---|---|---|
| Concept approval | | | | |
| Relationship approval | | | | |
| Versioning | | | | |
| Deprecation | | | | |
| Source mapping | | | | |
| Publication | | | | |

## Checklist

- [ ] Competency questions drive scope.
- [ ] Concepts are business-defined.
- [ ] Concepts and instances are distinguished.
- [ ] Relationships explicit and directional.
- [ ] Cardinality/constraints not invented.
- [ ] Context differences preserved.
- [ ] Evidence and ownership captured.
- [ ] Source mappings kept separate from semantic definitions.
- [ ] Governance/versioning considered.
- [ ] Data-product/AI use cases link to business value.
