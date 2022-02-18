# Thoughts re ATNS and sustainability

See video of the ATNS new website launch for background, history and aspirations of the ATNS: [https://www.youtube.com/watch?v=0q-OG0wsuN8](https://www.youtube.com/watch?v=0q-OG0wsuN8).

## Current System

### Social architecture?

  * who takes responsibility for keeping it running: now? future? Is it grant-dependant?
  * what governance processes govern it's usage, development, future?
  * what structures are established to communicate with users and potential information providers?
  * what intitutional and financial base underpins those processes?

### Technical architecture?

  * backend database: software?, schema?, scale?, how deployed? how managed? does it change? future plans?
  * frontend website: https://www.atns.net.au/ (squarespace?)
  * changes - how entered? how are relationships entered (e.g. associations between agreements and organisations)?
  * what is the technical debt, cost of running? Up to date? Secure? 
  * Is it at risk of becomeing an "orphan database" in future?

## Observations of current content

  * is this the current data capture form of the new site??: [https://www.atns.net.au/contact-us](https://www.atns.net.au/contact-us)
  * or does the old site data capture form still in play: [https://database.atns.net.au/lodge.asp](https://database.atns.net.au/lodge.asp)

[More information on content.](./content/00readme.md)
  
## Potential as a National Data Asset Stream 3 of ARDC

 * high level documentation of agreements of many types from many varied sources: very high policy/planning value to many parties;
 * do all agreements have a spatial component? If yes - GA may be a potential partner? If no, how can this be rectified?
 * relationships to legislation, organisations, jurisdictions etc.. -- very high potential for linked data;
 * "pointers" to external sources are sometimes text, sometimes URLs, sometimes 404's (not found/"link rot");
 * extremely high potential as a "use case" for information providers to support linked data and persistent identifiers

However, from observations based only exploring the front-end website, the resources in ATNS are human readable only (no embedded machine readable metadata beyond the whole of site level was evident afaict). This may be entirely misleading given the author's knowledge of the backend database in nil (appears to be a MS Access Database?).

In summary, the ATNS has high potential as a HAAS-I National Data Asset. 

The ATNS requires appropriate institutional level support for stimulating governance level discussions around:
   * what kind of things require "authoritative" and "persistent" machine readable identification (The ability to retain the integrity of those identifiers over time is important use case given the periods of time covered and the changing nature of the entities referenced). Examples:
      * organisations
      * agreements
      * .... etc TODO

Stimulating these kinds of discussions is entirely within the scope of the HASS-I/ARDC Indigenous Data Commons/Capability project.

## Towards an indigenous agreements ontology and knowledge graph?

If unfamiliar with the term, "knowledge graph", read [this](https://blog.cambridgesemantics.com/knowledge-graphs-origins-inhibitors-and-breakthroughs).

For applications of semantic web technology serving indigenous needs see [this paper by Aaron Corn](https://doi.org/10.1080/01576895.2019.1575248).

Potential formalised relationships and governance agreements:
 * National Native Title Tribunal (NNTT) (are there any formal data exchanges periodically?) Example pointer: [ilua:VI2010.003](http://www.nntt.gov.au/searchRegApps/NativeTitleRegisters/Pages/ILUA_details.aspx?NNTT_Fileno=VI2010/003) with ATNS equivalent entry: [atns:5303](https://www.atns.net.au/agreement?EntityID=5303). 
   * Important note: The atns entry contains a link to a PDF of the agreement on the NNTT site -- the link is broken. This is the core use case for why "persistent identifiers" and using them as a locator of important resources, is needed. 
 * Office of the Registrar of Indigenous Corporations (ORIC): [atsn:4626](https://www.atns.net.au/agreement?EntityID=4626)
 * many others e.g. ORIC, Aust Govt for formal Pids of Legislative instruments, AIATSIS re interoperability of high level subject categories and AUSLANG (Aiatsis Thesaurus and Indigenous Languages dataset).
 
Development of a high level ontology and movement by institutions which authoritatively manage the data to which ATNS refers towards persistent identifiers is about far more than about preventing broken links. An agreed ontology which describes the general categories which the ATNS provides relationships and linkages could provide a common framework for extending to a broader range of indigenous concerns where "agreements" are vital. The obvious one which comes to mind is the myriad of agreements implicit in the "Closing the Gap". An established ontology and semantic knowledge graph, which the ATNS may be a prime candidate case study to explore possibilities, could become a far more powerful service by allowing indigenous groups to extend such a KG with assertions describing their own experiences and aspirations e.g. successes, risks, barriers, achievements, exemplars etc.. 

Please note the above thoughts are purely speculative and "blue sky". They are offered to show the possibilities -- if institutional and social architectures can evolve to address classic "FAIR" concerns: Findability, Accessibility, Interoperability and Reusability in the overall context of Indigenous CARE principles. 
