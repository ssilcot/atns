# Thoughts re ATNS and sustainability

See video of the ATNS new website launch for background, history and aspirations of the ATNS: [https://www.youtube.com/watch?v=0q-OG0wsuN8](https://www.youtube.com/watch?v=0q-OG0wsuN8).

## Questions about the current ATNS system

### Social architecture and governance?

  * who takes responsibility for keeping it running: now? future? Is it grant-dependant?
  * what governance processes govern its usage, development, future?
  * what decision-making structures are established to communicate with users and potential information providers?
  * is ATNS coverage and accuracy part of someone's job?
  * what institutional and financial base underpins these processes?

### Technical and operational architecture?

  * backend database: software?, schema?, scale?, how deployed? how managed? does it change? future plans?
    * number of tables? physical size?
  * frontend website: https://www.atns.net.au/ (squarespace?)
    * approx number of query types (asp pages) supported by backend at https://database.atns.org.au/ ?
  * data updates - how entered? how are relationships entered (e.g. associations between agreements and organisations)?
    * volume of corrections? Any automated checking for broken links?
    * how many new agreements entered annually? updates? what is the process? quality assurance?
    * average time to respond to requests for corrections? for new agreements?
  * what is the technical debt, cost of running? Up to date? Secure? 
    * any active development?
  * Assessment of risk of becoming an "orphan database" in future?
    * what is required to secure ongoing operations and response to evolving opportunities?

## Observations of current content

  * is this the current data capture form of the new site??: [https://www.atns.net.au/contact-us](https://www.atns.net.au/contact-us)
  * or does the old site data capture form still in play: [https://database.atns.net.au/lodge.asp](https://database.atns.net.au/lodge.asp)

<!-- [More information on content.](./content/00readme.md)
-->

  
## Potential as a National Data Asset -- Stream 3 of ARDC Indigenous Data Capability Project

The ATNS website is properly designed for ease of human usage. There is no embedded machine readable metadata about each entry (e.g. RDFa or Json-LD). The database is accessible and returns html fragments.

Considering current ATNS contents:

 * it contains high level and high quality accurate documentation of agreements of many types from many varied sources: this has a very high policy/planning value to many parties;
   * coverage of agreements?
   * accuracy -- historical record? currency? records of amendment/change history?
 * do all agreements have a spatial component? If yes - GA may be a potential partner? If no, how can this be rectified?
 * relationships to legislation, organisations, jurisdictions etc.. -- very high potential for linked data;
 * "pointers" to external sources are sometimes text, sometimes URLs, sometimes 404's (not found/"link rot");
 * extremely high potential as a "use case" for information providers to support linked data and persistent identifiers

In summary, the **ATNS has very high potential value as a HAAS-I National Data Asset** in it's current form.

As an existing authoritative and comprehensive reference to Agreements of relevance to Indigenous communities it could easily be a source for Semantic Vocabularies (machine readable reference files hosted by the ARDC). These would provide a stable and persistent identity which can be used by other data producers to record theor own additional data about Agreements. For example, local Communities and researchers, could record their own observations about the success and effectiveness of Agreements, and share this data with others with no ambiguity about the particular Agreement being referred to. By encouraging the use of standard identifiers, the capability for Indigenous researchers to exchange, share and extend data about agreements is enhanced.

In addition, the possibility of enrichment with formal geospatial identifiers and geometries, and temporal/historical dimensions, would enable compatibility with the CSIRO's LOC-I framework. The ability to refer parties to Indigenous Agreements relevant to a location from the standard National Gazeteer and emerging services like the digital atlas of Australia is likely to be highly valued and welcomed by Geosciences Australia and CSIRO. 

It is very important to note that such developments can evolve using seperate Standard Vocabularies and external knowledge bases (e.g. RDF). These could provide for novel queries and visualisations where additional discursive explanations are obtained by pointing at the existing ATNS only when needed. This kind of evolution would not require significant change to the ATNS database per se, but it would require ATNS governance committments to:

 * ensure persistant identifiers are resolved to requests to resources for both humans and machines;
 * publish regular updates to Official Vocabularies and periodical database dumps to enable the knowledge graph to be refreshed with up to date content from time to time;
 * provide for logical deletion - deprecation rather than removal of inactive content;
 * attend to versioning and change history.


The ATNS requires appropriate institutional level support for stimulating governance level discussions around:

   * what kind of things require "authoritative" and "persistent" machine readable identification (The ability to retain the integrity of those identifiers over time is important use case given the periods of time covered and the changing nature of the entities referenced). 
   * Examples:
      * agreements (many different kinds, such as Framework Agreements from which other agreements are derived; this means agreements have meaningful relationships to each other -- is "related to" sufficient to reflect reality??)
      * organisations
      * legislative instruments
      * legal jurisdictions (determined by the State): international, national, state, LGAs etc.
      * indigenous "jurisdictions" (e.g. Coalition of Peaks)

Stimulating these kinds of discussions is entirely within the scope of the HASS-I/ARDC Indigenous Data Commons/Capability project.

## Can ATNS evolve to record new kinds of agreements?

Indigenous Data Sovereignty and Governance is a relevant issue. Yet there does not appear to a high level category in the ATNS Subject listing for these kinds of agreements? 

Why couldn't ATNS aspire to be a public record of agreements regarding indigenous data? Priority Four of Closing the Gap would appear to be an excellent opportunity for Indigenous data concerns to be well documented. Why not examine the feasibility of ATNS playing a role in disseminating that information to Indigenous Communities? 

At the very least, general framework agreements, principles and models of ID-GOV/ID-SOV which operationalise CARE principles can and should be recorded in ATNS. This possible evolution of the scope of the ATNS could be examined in the ARDC HASS-I National Data Assets work stream.

## Towards an indigenous agreements knowledge graph?

If unfamiliar with the term, "knowledge graph", read [this](https://blog.cambridgesemantics.com/knowledge-graphs-origins-inhibitors-and-breakthroughs).

For applications of semantic web technology serving indigenous needs see [this paper by Aaron Corn](https://doi.org/10.1080/01576895.2019.1575248).

Potential formalised relationships and governance agreements:

 * National Native Title Tribunal (NNTT) (are there any formal data exchanges periodically?) Example pointer: [ilua:VI2010.003](http://www.nntt.gov.au/searchRegApps/NativeTitleRegisters/Pages/ILUA_details.aspx?NNTT_Fileno=VI2010/003) with ATNS equivalent entry: [atns:5303](https://www.atns.net.au/agreement?EntityID=5303). 
   * Important note: The atns entry contains a link to a PDF of the agreement on the NNTT site -- the link is broken. This is the core use case for why "persistent identifiers" and using them as a locator of important resources, is needed. 
 * Office of the Registrar of Indigenous Corporations (ORIC): [atsn:4626](https://www.atns.net.au/agreement?EntityID=4626)
 * many others e.g. ORIC, Aust Govt for formal Pids of Legislative instruments, AIATSIS re interoperability of high level subject categories and AUSLANG (Aiatsis Thesaurus and Indigenous Languages dataset).
 
Development of a knowledge graph would require other institutions which authoritatively manage the data to which ATNS refers to adopt data governance practices which ensure links to their resources do not break (link rot). This is of course a longer term aspiration. 

A move towards persistent identifiers is about far more than about preventing broken links. An agreed ontology which describes the general categories which the ATNS provides relationships and linkages (i.e. the things it describes and points at) could provide a common framework for extending to a far broader range of indigenous concerns where "agreements" are vital. 

A formal ontology and vocabulary including classes of entities of concern to the ATNS, by providing a set of persistent identifiers about agreements and related parties, would assist Indigenous communities to describe their own experiences and aspirations e.g. successes, risks, barriers, achievements, exemplars etc. and explicitly associate those assertions with ATNS content. 

This kind of service could be of particular relevance in monitoring the impact and effectiveness of agreements.

## Agreements arising from Closing the Gap and Priority Item 4

One possible opportunity for the evolution of the ATNS would be as a preferred system of public record for the myriad of agreements implicit in the "Closing the Gap". Here is the [ATNS entry for the National Agreement](https://www.atns.net.au/agreement?EntityID=8063).

Is ATNS in it's current state able to function as a public record for ["place based" agreements](https://coalitionofpeaks.org.au/download/place-based-partnerships/) arising from Closing the Gap processes?

 * can Indigenous Communities negotiating these agreements register their own agreements data with the ATNS, or would data entry be required at the ATNS end? How sustainable is this? What is the current process for entering a new agreement and assigning it an identifier?
 * does the way "related agreements" are currently linked in the ATNS database capture appropriate meaning?
   * e.g. antecedents, precedents, place based instance of framework etc.?

Could ATNS aspire to be a provider of formal persistent identifiers for agreements - past and proposed - and provide an automated service in addition to the website to deliver machine readable core data? For example:

 * list/export all new agreements arising from framework agreement X within 1000km of my organisations's jurisdiction
 * list/export all new agreements about Land Use in Victoria
 * show all agreements including international jurisdictions which mention alcohol use in the last 3 years

Assuming that current Entity IDs can be ensured to be stable (via governance processes and committments about how the data is to be managed), could the current ATNS database system, or a separate derivative "knowledge graph" (just the core data about agreements - where, when, what, who, why - and their interrelationships) provide a useful service which can be pointed at by other systems e.g. [Closing the gap implementation tracker](https://www.closingthegap.gov.au/national-agreement/implementation-tracker)?

## Caveats

The above requires review arising from further information about current systems and aspirations of the ATNS's ownership. It is therefore vital to understand that the above thoughts are purely speculative. They are offered to explore possibilities which arise if institutional and social architectures can evolve to address classic "FAIR" concerns: Findability, Accessibility, Interoperability and Reusability in the overall context of Indigenous CARE principles. 

Committments to both:

 * sustaining ATNS in it's current role; 
 * exploring new roles for it with the aim of institutionalising it's ongoing funding and social/technical support  

will require attention to governance processes.

There is no doubt this resource is, and ought be managed as, a core National Indigenous Data Asset of primary concern. The fact that it only includes public information is a huge plus - a highly simplifying assumption in terms of technical degree of difficulty. However, the main challenges are of a governance and social architecture nature.

In the context of committments made in the context of Closing The Gap Priority Four (Data sharing) there would appear to be an opportunity for ATNS to evolve into a valued (and therefore funded and institutionalised) authoritative catalog of summaries of agreements concerning Indigenous people, including those involving indigenous data, which could exemplify both CARE and FAIR principles. 

Enhancing the ATNS's ability to provide information services for both humans and machines which authoritatively "point outwards" towards more detailed resources associated with those agreements would seem to be a "no-brainer".

## What does ATNS long term sustainability look like?

 * ongoing advocacy of the ATNS's long term strategic value as a National Indigenous Data asset
 * a plan for it's long term future which is feasible socially and technically
 * responsibility for custodianship by an institution which is committed to long term ATNS service operations and maintenance
   * this question could be explored as part of the ARDC HaSS-I project
 * established and transparent governance and decision making structures which are responsive to Community needs
 * operations, data collection and data quality processes which are designed to:
   * make it as easy as possible for Indigenous Communities to contribute high quality data;
   * make it as easy as possible for the Faculty of Law at Melbourne to continue to contribute high quality summaries;
   * maximise the client base and usefulness of the service; and 
   * minimise technical burden as far as is possible.
 * secure ongoing funding/support commensurate with the ATNS's national value which enables operational requirements and evolving Indigenous needs to be met.

Expansion of ATNS's scope to include **Indigenous Data Agreements, especially around Health, Medical and Genomic** related data collections, would be likely to increase the ATNS's chances of securing ongoing funding and support. 



 
