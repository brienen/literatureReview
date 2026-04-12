# Project: Systematic Literature Review MDIM

## Overzicht
Systematische literatuurstudie naar semantische interoperabiliteit in cross-domain publieke sector contexten, uitgevoerd volgens PRISMA 2020. Het doel is het identificeren van challenges, requirements en solutions voor het combineren van semantische domeinmodellen (Multi-Domain Information/semantic Models).

## Auteur
Arjen Brienen, TU Delft (abrienen@tudelft.nl)

## Werkruimten

### Literature Review MDIM (werkbibliotheek)
Gestructureerde PRISMA-werkmap met de volgende fases:
- `00_protocol/` — Protocol, criteria, amendments log
- `01_search/` — Query definities, zoekresultaten (Scopus, OpenAlex, Previous Studies)
- `02_deduplication/` — Ontdubbeling (leeg; vermoedelijk in Zotero afgehandeld)
- `03_abstract_screening/` — ASReview resultaten (CoreScreening en OpenAlex runs)
- `04_fulltext_screening/` — fullTextScreening.xlsx, eligibility_log, included fulltexts
- `05_coding/` — ATLAS.ti project, codebook, exports (Code Manager, Quotation Manager, XML)
- `06_synthesis/` — drafts, figures, tables (nog leeg)
- `10_logboek/` — Proceslogboek
- `99_python/` — Python omgeving (met .env)

### Article 2
Bevat het artikel in ontwikkeling. Twee parallelle lijnen:
1. "Framing Multi-Domain Semantic Conceptual Models" (v0.1 t/m v0.4.2, incl. commentaar Aaron en Marijn)
2. "Challenges, Requirements and solutions for semantic interoperability in the public sector" (v0.4.2 t/m v0.5.1)
Inclusief Omnigraffle-diagrammen (Interoperability Challenges, Requirements, Solutions).

### Zotero
Volledige Zotero-database. Relevante bibliotheken:
- **Library 1 (User library):** Persoonlijke hoofdbibliotheek ("Core knowledge"), NIET AANPASSEN
- **Library 3 (LitReview):** Eerdere review-bibliotheek met thematische collecties (Government Semantic Interoperability, etc.), 1307 items, 396 annotaties
- **Library 5 (LiteratureReviewMDIMs):** Actieve werkbibliotheek voor deze review, 4141 items
  - Bevat PRISMA-workflow collecties: 00_RAW Input → 01_Abstract_Screening → 02_FullText_Assessment → 03-Snowballing
  - Twee screeningstromen: CoreScreening (Scopus) en OpenAlex
  - Tags: LR_Query, LR_SearchDate, ASReview labels (Relevant/Irrelevant), exclusiecriteria (EC1 t/m EC6)

## Veiligheidsregels Zotero
- **Maak ALTIJD een backup voordat je wijzigingen aanbrengt in de Zotero database**
- Werk uitsluitend in de groepsbibliotheek "LiteratureReviewMDIMs" (library 5)
- De hoofdbibliotheek (library 1) is Core Knowledge en mag niet gewijzigd worden

## Schrijfconventies
- Gebruik geen tussenstreepjes in lopende tekst; gebruik komma, puntkomma of dubbele punt
- Academische schrijfstijl, Engels voor het artikel, Nederlands voor procesnotities

## Codebook
Het codebook volgt het European Interoperability Framework (EIF) met vier lagen:
- Challenges (CH): Semantic, Technical, Organizational, Legal
- Solutions (SOL): bijbehorende oplossingsrichtingen
- Requirements (REQ): vereisten voor semantische interoperabiliteit
Subcategorieën worden getagd met #-notatie (bijv. #SEM_ConceptualDivergence, #CH-Technical)

## Fase en status
- Zoeken: afgerond (Scopus jan 2026, OpenAlex mrt/apr 2026)
- Abstract screening: afgerond via ASReview (twee stromen)
- Full-text screening: in uitvoering (fullTextScreening.xlsx)
- Codering: begonnen in ATLAS.ti (codebook ontwikkeld, kernartikelen geannoteerd)
- Synthese: nog niet gestart

## Technische context
- Zotero database: SQLite (`zotero.sqlite`), read-only via Python sqlite3
- ASReview voor abstract screening
- ATLAS.ti voor kwalitatieve codering
- Obsidian als notitiemethode (vault in Literature Review MDIM)
- Python omgeving in 99_python/
