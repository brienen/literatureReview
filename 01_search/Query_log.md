---
title: "Query Log"
description: "Logbestand voor het systematisch vastleggen van uitgevoerde zoekopdrachten per databank, conform PRISMA-richtlijnen."
created: 2026-01-15
maintained_by: "Arjen Brienen"
---

## Doel

Dit bestand registreert **alle daadwerkelijk uitgevoerde zoekopdrachten**, inclusief datum, databank, exacte query, toegepaste filters en het aantal resultaten. Het fungeert als audit trail voor transparantie en reproduceerbaarheid van de literatuursearch.

## Query-overzicht

| ID  | Datum      | Databank       | Query (samengevat)                        | Filters / Limieten        | # Resultaten                        | Export | Opmerkingen     |                                 |
| --- | ---------- | -------------- | ----------------------------------------- | ------------------------- | ----------------------------------- | ------ | --------------- | ------------------------------- |
| Q1  | 2026-01-15 | Scopus         | Semantic interoperability & domain models | Zie `queries.md` §Scopus  | Subject areas: CS, IS; Language: EN | 243    | `scopus_Q1.csv` | Initiële brede search           |
| Q2  | 2026-01-15 | Web of Science | Semantic interoperability & domain models | Zie `queries.md` §WoS     | Categories: CS, PA; Language: EN    | 198    | `wos_Q2.xlsx`   | Licht smaller bereik            |
| Q3  | 2026-01-15 | Google Scholar | Semantic interoperability & public sector | Zie `queries.md` §Scholar | Since 2005; Sort by relevance       | ~320   | n.v.t.          | Indicatief, handmatig gescreend |

## Kolomdefinities

- **ID** – Unieke identificatie van de zoekactie (Q1, Q2, …).
- **Datum** – Datum waarop de query is uitgevoerd.
- **Databank** – Gebruikte bron (bijv. Scopus, Web of Science, Google Scholar).
- **Query (samengevat)** – Korte menselijke omschrijving van de zoekstrategie.
- **Filters / Limieten** – Toegepaste filters (jaar, taal, vakgebied, documenttype).
- **# Resultaten** – Aantal hits zoals gerapporteerd door de databank.
- **Export** – Bestandsnaam van de geëxporteerde resultaten (indien van toepassing).
- **Opmerkingen** – Relevante context (bijv. reden voor herhaling, aanpassing t.o.v. eerdere query).

## Wijzigingen en heruitvoering

Bij aanpassing of heruitvoering van een query:
- voeg een **nieuwe rij** toe;
- verwijs in *Opmerkingen* expliciet naar het eerdere Query-ID;
- documenteer **wat** is gewijzigd en **waarom**.

Dit voorkomt overschrijven van zoekgeschiedenis en ondersteunt PRISMA-amendments.