---
title: "Protocol Amendments Log"
project: "Semantic Interoperability Review"
author: "Arjen Brienen"
affiliation: "Delft University of Technology"
status: "active"
prisma_version: "PRISMA 2020"
date_created: 2026-01-15
last_updated: 2026-04-12
---

# Protocol amendments log

This document records all amendments to the review protocol that occur after the commencement of the systematic literature review. It serves as a transparent audit trail in accordance with PRISMA 2020. Amendments are documented chronologically and are not retroactively applied to earlier stages unless explicitly stated.
## Amendment entries

### Amendment A1
- **Date:** 2026-04-12
- **Protocol element affected:** Full-text eligibility assessment procedure
- **Description of change:**
  The original protocol (Section 6) specifies that full-text eligibility is assessed using the predefined exclusion criteria EC1 through EC6 (as documented in [[Criteria]]). This amendment introduces a structured quality and relevance scoring instrument as the primary mechanism for inclusion and exclusion decisions at the full-text stage. Each article is assessed on four dimensions, each scored on a three-point scale (0, 1, 2):

  **A. Topical Relevance (0–2):** The extent to which the article substantively addresses semantic interoperability in public-sector or cross-organizational contexts.
  **B. Analytical Contribution (0–2):** The type of analytical contribution beyond description, including whether the article links challenges to requirements, principles, or solutions.
  **C. Level of Abstraction and Transferability (0–2):** The extent to which insights are abstracted from the specific empirical context and articulated in a reusable form.
  **D. Conceptual and Methodological Rigor (0–2):** The clarity and coherence of conceptual and methodological grounding.

  The four dimension scores are summed to produce a total score (range 0–8). Inclusion and exclusion are determined as follows:

  - **Included:** Total score ≥ 7. The article makes a sufficient contribution across relevance, analytical depth, transferability, and rigor to warrant inclusion in the qualitative synthesis.
  - **Excluded on score:** Total score < 7. The article does not meet the combined quality and relevance threshold for inclusion.
  - **Excluded on knock-out:** Regardless of score, an article is excluded if it meets any of the exclusion criteria EC1–EC6, or if the full text is not available or not in English. Knock-out exclusions are recorded separately from score-based exclusions.

  The scoring criteria, including detailed definitions and scoring anchors for each dimension, are specified in the "Full text Scoring Criteria" section of [[Criteria]].

  *Note:* The minimum inclusion threshold of 7 is subject to revision as screening progresses. Any change to this threshold will be documented as a separate amendment (see A2 reserved).

- **Rationale:**
  During full-text assessment, it became apparent that the binary application of exclusion criteria (EC1–EC6) was insufficient to distinguish between articles that vary considerably in their contribution to the review objectives. Many articles address semantic interoperability in a public-sector context (and therefore do not trigger any EC criterion) yet differ substantially in analytical depth, level of abstraction, and methodological rigor. A structured scoring instrument provides a transparent, reproducible, and auditable basis for these distinctions, reduces subjective variability in inclusion decisions, and enables sensitivity analysis by adjusting the threshold post hoc.

- **Stage of review:**
  During full-text eligibility assessment.

- **Impact on results:**
  This amendment changes the operationalization of full-text screening from a purely criteria-based approach to a combined criteria and scoring approach. The scoring instrument does not replace EC1–EC6; rather, it complements the exclusion criteria by providing a structured basis for inclusion decisions among articles that pass the knock-out check. The threshold determines the boundary between included and excluded studies: at the current threshold of 7, the CoreScreening stream yields 35 included articles out of 91 scored articles. Adjusting the threshold would directly affect the number of included studies and should be assessed for its impact on the representativeness and breadth of the synthesis.

- **PRISMA reporting note:**
  The PRISMA flow diagram should report the number of full-text articles excluded, distinguishing between (a) knock-out exclusions citing EC criteria or accessibility issues, and (b) score-based exclusions below the inclusion threshold. The Methods section should describe the scoring instrument, the four dimensions, the scoring anchors, and the applied threshold. The full scoring results per article are recorded in `fullTextScreening.xlsx`.

## Guidance for use

Amendments are recorded only after the protocol has been finalized. Editorial clarifications without methodological impact are not logged. Each amendment receives a unique identifier (A1, A2, …). If an amendment introduces an additional search wave, this is reflected consistently in `search_log.xlsx`, screening outputs, and PRISMA flow reporting. This document is version-controlled and should not be rewritten retrospectively.
## Relationship to other artefacts

- [[protocol]] documents the a priori methodological design.
- [[query]] specifies the intended search logic.
- [[Query_log]] records the execution of searches.
- [[eligibility_log]] records full-text inclusion and exclusion decisions.

Together, these artefacts provide a complete and auditable account of methodological decisions.