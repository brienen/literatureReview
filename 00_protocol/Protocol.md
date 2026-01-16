---
title: "Systematic Literature Review Protocol"
project: "Semantic Interoperability Review"
author: "Arjen Brienen"
affiliation: "Delft University of Technology"
status: "approved"
prisma_version: "PRISMA 2020"
date_created: 2026-01-15
last_updated: 2026-01-15
---

# Review protocol

This document specifies the **a priori protocol** governing the systematic literature review.
It defines the methodological choices for search, screening, eligibility assessment, coding, and synthesis, in accordance with PRISMA 2020.

Once screening has commenced, this protocol is considered fixed.
Any deviations are documented in [[Amendments_log]].

## 1. Background and rationale

Semantic interoperability is widely recognized as a structural barrier to data sharing and coordinated policy implementation in the public sector. Despite the proliferation of domain-specific information models and semantic standards, systematic insight into how semantic models can be combined across domains remains limited.

This review aims to synthesize academic literature addressing semantic interoperability challenges and solution approaches, with particular attention to conceptual, organizational, and governance-related aspects.

## 2. Objectives and research questions

The objective of this review is to identify and synthesize academic literature on semantic interoperability in cross-domain public-sector contexts.

The review addresses the following research questions:

- What types of semantic interoperability challenges are identified in the literature?
- What solution constructs or approaches are proposed to address these challenges?
- What requirements are articulated for combining semantic domain models?

## 3. Review scope

- **Phenomenon of interest**: semantic interoperability and shared meaning across information systems.
- **Analytical focus**: conceptual and semantic artefacts such as information models, ontologies, and domain models.
- **Context**: public-sector, governmental, or policy-related settings.
- **Perspective**: cross-organizational and cross-domain interoperability.

## 4. Information sources

The primary information sources are bibliographic academic databases:

- Web of Science
- Scopus

Grey literature may be consulted in a supplementary manner where it provides authoritative conceptual or policy insight. Such sources are explicitly documented and reported separately.

## 5. Search strategy

Search strategies are designed for high recall and are specified in [[Query]].
Queries are adapted to the syntax of each database but preserve conceptual equivalence.

Search execution details, including dates, filters, and result counts, are recorded in [[Query_log]].

## 6. Study selection process

The study selection process follows PRISMA 2020 and consists of the following stages:

1. Import of retrieved records into a reference manager.
2. Deduplication with preservation of source provenance.
3. Title and abstract screening using active-learning–supported screening software.
4. Full-text eligibility assessment based on predefined criteria.

Reasons for exclusion at the full-text stage are documented in [[eligibility_log]].

## 7. Eligibility criteria

Eligibility criteria are defined a priori and documented in [[Inclusion_criteria]].

During abstract screening, criteria are applied conservatively to maximize recall.
During full-text assessment, all criteria are applied in full.

## 8. Data extraction and coding

Eligible studies are subjected to qualitative coding using a predefined, theory-informed codebook.

- Coding is conducted in a dedicated qualitative analysis environment.
- The codebook is refined iteratively during early coding stages.
- Codebook snapshots are exported at analytically meaningful milestones.

Exported codebooks and analytic summaries are versioned as research artefacts.

## 9. Synthesis approach

The review employs a qualitative, thematic synthesis.

Synthesis focuses on:
- recurring challenge types,
- solution constructs,
- articulated requirements for semantic model combination.

The emphasis is on conceptual patterns and explanatory insights rather than quantitative aggregation.

## 10. Reproducibility and data management

All methodologically relevant artefacts, including queries, logs, screening outputs, and analytic exports, are stored in a version-controlled repository.

Internal databases of proprietary tools are excluded; only exported snapshots are retained to ensure auditability and reproducibility.

## 11. Protocol amendments

Any amendments to this protocol after the commencement of screening are recorded in `amendments_log.md`, including the rationale and implications for the review.