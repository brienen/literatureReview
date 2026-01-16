---
title: "Queries – Scopus, Web of Science, Google Scholar"
description: "Eén samengestelde zoekquery per bibliotheek (Scopus, Web of Science, Google Scholar) voor literatuur over het combineren van (semantische) domeinmodellen over domeinen heen en interoperabiliteit in de publieke sector."
created: 2026-01-15
---

## Scopus queries

Plak in **Scopus Advanced Search**
### Scopus_2
Core Minimal Viable Query, around 400 hits 

```
TITLE-ABS-KEY(
  (
    "semantic interoperability"
    OR ("semantic" W/2 (interoperab* OR integrat* OR align*))
    OR ("semantic web" AND interoperab*)
    OR "cross-domain"
    OR "cross domain"
    OR "multi-domain"
    OR "multi domain"
  )
  AND
  (
    ontolog*
    OR "information model*"
    OR "domain model*"
    OR "data model*"
    OR "metadata model*"
    OR "semantic infrastructure*"
    OR "thesaur*" OR "taxonom*" OR "controlled vocabular*"
  )
  AND
  (
    "public sector"
    OR "public administration"
    OR government
    OR "e-government"
    OR egov*
    OR "open government data"
    OR "public service*"
    OR "european union"
    OR EU
  )
)
AND PUBYEAR > 1999 AND (LIMIT-TO(LANGUAGE, "English"))
```

### Scopus_1
Full scopus query max coverage but 2000+ hits

```
(
  TITLE-ABS-KEY(
    "semantic interoperability"
    OR "semantic alignment"
    OR "semantic integration"
    OR "shared semantics"
  )
  OR
  TITLE-ABS-KEY(
    ("ontology" OR "ontologies" OR "upper ontology" OR "core ontology"
 OR "thesaur*" OR "taxonomy" OR "controlled vocabular*"
 OR "concept scheme" OR "information model*" OR "data model*"
 OR "knowledge graph*" OR "knowledge base*"
 OR "semantic model*" OR "domain model*"
 OR "conceptual schema*"
 OR "semantic mapping*" OR "ontology alignment*"
 OR "knowledge representation")
    AND (interoperability OR integration OR harmonization OR "multi domain" OR "multi-domain")
  )
)
AND (
TITLE-ABS-KEY(
  government
  OR "public sector"
  OR "public administration"
  OR "public authorit*"
  OR municipalit*
  OR "local government"
  OR "regional government"
  OR "provincial government"
  OR province*
  OR "state government"
  OR "national government"
  OR "central government"
  OR "federal government"
  OR intergovernmental
  OR "european union"
)
)
AND PUBYEAR > 1999 AND ( LIMIT-TO ( LANGUAGE , "English" ) )
```


## Web of Science queries

### Web_1

```
To be done
```

## Google Scholar queries

```
To be done
```
