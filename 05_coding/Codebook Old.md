# Codebook (MDIM literatuurstudie)

### Methodological Note  
The challenge categories in this codebook are aligned with the four interoperability layers defined by the European Interoperability Framework (EIF). While the EIF provides a structural distinction between legal, organizational, semantic and technical layers, it does not define operational coding criteria. The definitions and coding rules used here are therefore derived from scientific literature in information systems, semantic technologies, e-government and organizational studies.  

Definitions were developed by synthesizing conceptual descriptions from foundational studies (e.g., Sheth & Larson 1990; Bowker & Star 1999; Euzenat & Shvaiko 2013; Scholl & Klischewski 2007) and translating them into operational coding criteria based on recurring empirical patterns such as divergent meaning structures, incompatible interfaces, misaligned business processes, or conflicting regulatory requirements.  

Inclusion criteria specify when a text fragment should be assigned to a category, while exclusion criteria prevent overlap between categories by distinguishing semantic, technical, organizational and legal sources of interoperability problems. These criteria aim to ensure analytical clarity, reproducibility and theoretical grounding.

Main catagorization is done in color, sub-categorization is done using tags. All categories match the EIF (European Interoperability Framework)[^eif] 

## Challenges (Orange)
These categories align with the four interoperability layers defined by the EIF, while the definitions and coding criteria are derived from scientific literature on semantic, technical, organisational and legal interoperability.

### #CH-Semantic
**Literature**: 
Wat ik in literatuur vind om te classificeren:
1. Park (2004), "Information Systems Interoperability: What Lies Beneath?": Is more about database design data-level (entity- vs attribute-level) en schema-level conflicts (naming, entity-identifier, Schema-isomorphism, Generalization conflicts, Aggregation conflicts, Schematic discrepancies) 
2. Vogt (2024), "FAIR 2.0: Extending the FAIR Guiding Principles to Address Semantic Interoperability": Based on natural language study. introduces: 
	1. referential interoperability, 
	2. Terminological interoperability, 
	3. Propositional interoperability (semantic interoperability of statements), 
		1. "logical interoperability only depends on whether reasoning operations  can be applied to the data. It does not necessarily include that the data are also logically consistent."
		2. Schema interoperability (one schema or mapping(crosswalks))
3. Tolk (2003), "The Levels of Conceptual Interoperability Model": Levels: 
	1. Level 0 - System Specific Data  No interoperability between two systems. Data is used within each system in a proprietary way with no sharing. The component (or application) is a black box.
	2. Level 1 – Documented Data  Data is documented using a common protocol, such as the Object Model Template defined by the HLA and is accessible via interfaces. The component is a black box with an interface.
	3. Level 2 – Aligned Static Data  Data is documented using a common reference model based on a common ontology, i.e., the meaning of the data is unambiguously described.
	4. Level 3 – Aligned Dynamic Data  The use of the data within the federate/ component is well defined using standard software engineering methods such as UML.
	5. Level 4 – Harmonized Data  Semantic connections between data that are not related concerning the execution code is made obvious by documenting the conceptual model underlying the component.
4. Guarino (1998) "Formal Ontology and Information Systems". introduction to conceptualization. & Coarse vs. fine-grained ontologies & The Ontology Integration Problem "The quantity of ontological knowledge available may be modest, but it is its quality, i.e. the nature of some fundamental ontological distinctions, which can help the designer in his task of conceptual analysis." 
5. Euzenat & Shvaiko (2013)"Ontology Matching", defines heterogeneity: Syntactic heterogeneity, Terminological heterogeneity, Conceptual heterogeneity and Semiotic heterogeneity (semiotic is moeilijk voor computers te begrijpen dus deze wordt niet behandeld). 


**Definition**: Semantic interoperability concerns the shared interpretation and consistent meaning of data across organisations. Challenges arise when the underlying conceptual structures, meaning assumptions or representational conventions diverge across domains.
**Inclusion**:
  - #SEM_Syntax Semantic interoperability challenge arising when semantic models or information artefacts are expressed using different representation or formal languages, such that their structures or constructs are not directly comparable without explicit translation or mapping. (Euzenat & Shvaiko 2013, p37)
  - #SEM_UnderspecifiedMeaning Semantic interoperability challenge arising when relevant concepts, properties, or relations are insufficiently, or not at all, conceptualized or left implicit, such that the meaning of data or information artefacts cannot be reliably interpreted or related to real-world phenomena. This includes situations where semantic content remains embedded in unstructured, weakly structured, or fragmented representations. _Guarino, N. (1998). Formal ontology and information systems_. (Euzenat & Shvaiko 2013, p38)
  - #SEM_ConceptualDivergence Semantic interoperability challenge arising from differences in how entities, attributes, or relations are conceptualized, such that modeling assumptions about meaning, granularity, or scope are misaligned, even when referring to comparable phenomena. This includes non-equivalence caused by mismatched levels of abstraction and divergent meaning structures that lead to inconsistent interpretation, rather than differences between problem domains as such. Vogt (2024), (Euzenat & Shvaiko 2013, p38)
  - #SEM_DataHeterogeneity  Semantic interoperability challenge arising when problem domains differ in applications, scope, boundaries, or underlying assumptions, such that meanings are not directly comparable or transferable across domains. These differences exist independently of whether domains are explicitly conceptualized or remain implicit. When persistent, such heterogeneity contributes to the formation of semantic silos.
  - #SEM_ExpressivenessLimit Semantic interoperability challenge arising from limitations in the expressive power or representational adequacy of ontology-based formalisms, where formal structures such as class hierarchies cannot fully or faithfully capture complex, fuzzy, or context-dependent meanings.
  - #SEM_DataQuality Semantic interoperability challenge arising when data contain errors or otherwise fail to accurately convey their intended meaning, resulting in inconsistent interpretation, reduced usability, or loss of conceptual fidelity across contexts (Vogt, 2024).
  - #SEM_MuliLanguage Semantic interoperability challenge arising from differences in natural languages (ie. English, Dutch or Swedish) used to label, describe, or document data and models, leading to ambiguity, translation loss, or inconsistent interpretation across linguistic contexts. 
  - #SEM_MetadataInsufficiency Semantic interoperability challenge arising when metadata are incomplete, inaccurate, or missing, such that the meaning, context, or constraints of data cannot be reliably understood or interpreted. [^aliDevelopmentInteroperableOpen2024]  
**Exclusion**:
  - purely technical issues concerning formats, APIs or protocols
  - legal constraints not affecting meaning
  - organizational constraints not affecting meaning

## #CH-Technical
**Definition**
Technical interoperability concerns the ability of applications and underlying infrastructures to connect systems and services in a reliable and machine-processable manner. It covers the technical mechanisms that enable data presentation, exchange, and integration, including interface specifications, interconnection services, data integration services, and secure communication protocols. Technical challenges arise when these mechanisms are fragmented, incompatible, or insufficiently implemented, thereby obstructing effective system-to-system interoperability.
**Inclusion**
- #TECH_IncompatibleTechnique incompatibilities in system architectures, platforms, or infrastructure, including constraints imposed by legacy systems
- #TECH_Interface absence, partial adoption, or inconsistent implementation of shared technical standards for data exchange, interfaces, or services
- #TECH_Transport limitations in discoverability, data transport, service connectivity, authentication, or authorization mechanisms that hinder secure and stable communication
- #TECH_MachineReadable failures in syntactic validation, schema conformance, or machine-level processability of exchanged data
**Exclusion**
- differences in meaning, interpretation, or conceptualisation of data elements or structures (semantic layer)
- misalignment of organisational roles, responsibilities, workflows, or governance arrangements (organisational layer)
- legal or policy constraints that restrict data exchange independently of technical feasibility

## #CH-Organizational 
Definition: Organisational interoperability concerns the alignment of business processes, governance structures, roles and responsibilities needed to coordinate joint service delivery across organizations. _Compare with Maheshwari, D., & Janssen, M. (2012). Government Information Quarterly, 29(3). page 6_
Inclusion:
- #ORG_Capacity Organizational interoperability challenge arising from insufficient structural capacity, including lack of time, funding, staffing, or institutional support to implement and sustain interoperability solutions.
- #ORG_Overhead Organizational interoperability challenge caused by the coordination, governance, and management overhead required to align multiple organizations, processes, and responsibilities, where the organizational effort itself becomes a bottleneck to interoperability. **Zou gezien kunnen worden als een capaciteitsprobleem dat ontstaat door de inzet op interoperabiliteit**
- #ORG_Expertise Organizational interoperability challenge arising from insufficient domain, semantic, or technical expertise required to design, implement, interpret, and sustain interoperability solutions, including structured semantic data, ontologies, and linked data. complexity issues and lack in ability of people and organizations to cope with complex issues 
- #ORG_Agreement Organizational interoperability challenge arising from the absence of shared organizational agreements on the interpretation and use of semantic concepts across public service providers, despite the availability of common models or standards. Dit betreft afspraken over organisatorische eenheden heen. **Zou overlap met #ORG_Governance kunnen hebben omdat het een tekort aan governance afspraken betekent**  
- #ORG_Governance Organizational interoperability challenge arising from the absence of explicit governance, ownership, or managerial steering for semantic interoperability, resulting in semantic issues being handled ad hoc within technical or business silos. Like: misaligned or incompatible business processes that prevent end‑to‑end service delivery (Scholl & Klischewski 2007), unclear distribution of roles, responsibilities or decision rights and lack of coordination mechanisms, collaboration structures or shared governance arrangements
- #ORG_Instrumentarium Organizational interoperability challenge arising from the absence or insufficient availability of appropriate tools, methods, and operational practices required to design, implement, manage, or apply interoperability and semantic solutions.
- #ORG_Diversity Organizational interoperability challenge arising from persistent differences in organizational structures, roles, responsibilities, and management processes across public administrations, which hinder alignment and increase the effort required for interoperability.
- #ORG_Culture Organizational interoperability challenge arising from prevailing organizational values, norms, attitudes, and practices that discourage, deprioritize, or resist interoperability, data sharing, or semantic alignment, even when governance structures, expertise, and instruments are formally in place.
Exclusion:
  - purely technical integration problems
  - semantic divergences unrelated to process structures
  - legal barriers arising from incompatible regulatory frameworks

## #CH-Legal 
Definition: Legal interoperability concerns the extent to which binding legal instruments enable, constrain, or structurally condition interoperability across domains and organizations.
Inclusion:
  - #LEG_Incompability Varying or incompatible legal requirements. such as conflicting legislative requirements that hinder data exchange (Weber 2019)
  - #LEG_Restrictions or jurisdictional restrictions on data access, storage or reuse. Including privacy restrictions. 
  - #LEG_Licensing incompatible licensing regimes or data ownership rules
  - #LEG_Clarity Lack of legal clarity regarding responsibilities, rights or liabilities in shared-service arrangements. _Supported by Scholl & Klischewski (2007)_
  - #LEG_instability This subtype concerns situations where laws, regulations, or policy criteria are subject to frequent modification, reinterpretation, or re-scoping, thereby undermining shared understandings, durable semantic agreements, and stable implementation practices.
  - #LEG_Overhead Legal interoperability challenge arising from the juridical and governance burden of establishing, negotiating, and maintaining multilateral agreements to mandate shared standards, where the agreement process itself becomes a bottleneck to interoperability. _Supported by Kubicek, Cimander & Scholl (2011)_
Exclusion:
  - semantic or technical challenges not rooted in law
  - organizational misalignment unrelated to regulatory constraints

## Solution Types (Green)

### #APP-Ontology  
Definition: Approaches that use formal ontologies to structure, represent or integrate domain knowledge, typically using Linked Data standards (e.g., RDF, OWL). Ontology-based approaches aim to achieve semantic precision, interoperability, and machine-readable meaning structures.  
Inclusion:  
  - use of RDF/OWL/Turtle models  
  - creation or reuse of domain ontologies  
  - ontology-driven integration or reasoning  
  - semantic graph representations enabling alignment  
Exclusion:  
  - simple controlled vocabularies without formal semantics  
  - metadata-only alignment without ontology structure

### #APP-SemanticAlignment  
Definition: Approaches focused on semantic alignment between heterogeneous models, vocabularies or data sources. These methods aim to reduce conceptual heterogeneity.  
Inclusion:  
  - ontology mapping techniques  
  - schema or vocabulary harmonisation  
  - semantic mediation or matching  
  - creation of crosswalks or equivalence mappings  
Exclusion:  
  - purely technical transformation (e.g., ETL)  
  - organizational negotiations without semantic content

### #APP-DataReferenceModel  
Definition: Approaches that define a standardised set of data elements, categories or structures used across domains to support alignment and reuse. Data Reference Models provide only partial standardization on specific data elements    
Inclusion:  
  - domain-independent data element models  
  - reference data structures for cross-domain exchange  
  - authoritative definitions of core entities  
Exclusion:  
  - free-form glossaries without structural constraints  
  - domain-specific models not intended as reference standards
Examples:
- EU Core Vocabularies

### #APP-DataDictionary  
Definition: Approaches that provide shared definitions, descriptions and permissible values for data elements without prescribing a full conceptual structure.  
Inclusion:  
  - shared term lists with definitions  
  - controlled vocabularies  
  - standardized descriptions of fields or attributes  
Exclusion:  
  - full ontologies or conceptual models  
  - unstructured lists without definitional clarity

### #APP-CommonDataModel  
Definition: Approaches that introduce a unified, shared data model used by multiple organisations or domains to harmonise data exchange and integration.  
Inclusion:  
  - single canonical data models used across systems  
  - harmonised schemas supporting interoperability  
  - models replacing divergent local structures  
Exclusion:  
  - federated or decentralised approaches  
  - mappings without adoption of a common model


### #APP-Federated  
Definition: Approaches in which multiple independently maintained models or systems interoperate through mappings, mediation or shared protocols rather than through a single unified model.  
Inclusion:  
  - federated ontology architectures  
  - model-to-model mappings enabling local autonomy  
  - distributed governance structures  
Exclusion:  
  - enforced use of one centralised data model  
  - purely technical federation without semantic alignment


### #APP-MetaData  
Definition: Approaches that align or standardise metadata schemas to ensure data is findable, understandable and reusable across organisations and systems.  
Inclusion:  
  - metadata schema harmonisation  
  - use of standards such as DCAT, Dublin Core, schema.org  
  - cross-domain metadata interoperability  
Exclusion:  
  - semantic alignment of domain concepts (belongs in APP-SEM)  
  - metadata limited to local documentation without interoperability intent

## Different Government Domains (Blue)
definition: government policy domains, or fields where semantic interoperability challenges are found or approaches can be implemented 


## Previous relevant studies (Purple)
definition: studies that directly address challenges of (semantic) interoperability and approaches  


## Preconditions for semantic interoperability (Magenta)
definition: things taht need to be met in order to facilitate (semantic) interoperability




## References  
Bowker, G. C., & Star, S. L. (1999). *Sorting things out: Classification and its consequences*. MIT Press.  

Euzenat, J., & Shvaiko, P. (2013). *Ontology matching*. Springer.  

Gruber, T. R. (1995). Toward principles for the design of ontologies used for knowledge sharing. *International Journal of Human–Computer Studies, 43*(5–6), 907–928.  

Halevy, A., Rajaraman, A., & Ordille, J. (2006). Data integration: The teenage years. In *Proceedings of the 32nd International Conference on Very Large Data Bases* (pp. 9–16).  

Maheshwari, D., & Janssen, M. (2014). Reconceptualizing measuring, benchmarking for improving interoperability in smart ecosystems: The effects of smart governance and smart environment. *Government Information Quarterly, 31*(Supplement 1), S84–S94.  

Scholl, H. J., & Klischewski, R. (2007). E-government integration and interoperability: Framing the research agenda. *International Journal of Public Administration, 30*(8–9), 889–920.  

Sheth, A. (1999). Changing focus on interoperability in information systems: From system, syntax, structure to semantics. In M. F. Worboys & M. Duckham (Eds.), *Interoperating geographic information systems* (pp. 5–29). Springer.  

Sheth, A., & Larson, J. (1990). Federated database systems for managing distributed, heterogeneous, and autonomous databases. *ACM Computing Surveys, 22*(3), 183–236.  

Weber, R. H. (2019). Legal interoperability as a tool for combatting fragmentation. *European Journal of Law and Technology, 10*(3).  

European Commission. (2017). *New European interoperability framework: Promoting seamless services and data flows for European public administrations*. Publications Office of the European Union. https://doi.org/10.2799/78681

[^aliDevelopmentInteroperableOpen2024]: 