---
layout: page
title: Projects
permalink: /projects/
nav_order: 6
---

<style>
table th:first-of-type {
    width: 20px;
}
table th:nth-of-type(2) {
    width: 20px;
}
</style>

{: .highlight-title }
> 🚧 Under Construction
>
> This page is still being developed. [Contact us](/metadata-documentation/contact/) with any questions or feedback.

# Projects
{: .no_toc }

An overview of projects initiated by or involving the Metadata Services Unit (MSU) and other collaborators throughout the Library

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Active

---

Last updated September 2023
{: .float-right .fs-2 .text-grey-dk-000 }
### Schomburg Art & Artifacts MARC Records

| Dates | beginning January 2023 |
| Collaborators | Schomburg Art & Artifacts; BookOps; Special Collections Processing |

#### Overview
{: .no_toc }

- Schomburg Art and Artifacts Division provided SCP and MSU twelve spreadsheets containing description for items within their collection based on formats including:  Artifacts, Buttons, Calendars, Drawings, Medals, Paintings, Portfolios, Postcards, Posters, Prints, Sculptures, and Textiles
- MSU is editing, updating, and standardizing the metadata, including locating the Library of Congress Name Authorities for applicable names and corporations and determining mapping between this metadata and MARC fields
- MSU and BookOps are creating a [Python script 🔒](https://github.com/NYPL/metadata-projects/tree/main/in-progress/2023-02_schomburg_art_artifacts_marc_records) to create MARC records from the updated metadata
- These MARC records will be loaded into Sierra and imported into MMS where applicable

---

Last updated September 2023
{: .float-right .fs-2 .text-grey-dk-000 }
### Name Element & Name Subject URIs

| Dates | beginning August 2020 |
| Collaborators | Access Services; SASB Periodicals Section; General Humanities Operations; Preservation of Audio and Moving Image |
| Related Links | [Matching text names with authority headings (Instructional Google Slides) 🔒](https://docs.google.com/presentation/d/1jp9h37IKKxhty_eQ7rp-AoXIyhkLzzDxtiTLpRHk7wI/edit){: .btn } [Name Element Tracking (completed) 🔒](https://docs.google.com/spreadsheets/d/1WkZyQmBLmLsafPE-RsOooIwLLNSRBLG99q5RD9G5Bts/edit#gid=0){: .btn } [Name Subject Element Tracking (in progress) 🔒](https://docs.google.com/spreadsheets/d/1WkZyQmBLmLsafPE-RsOooIwLLNSRBLG99q5RD9G5Bts/edit#gid=2100468148){: .btn } |

#### Overview
{: .no_toc }

- When COVID-19 required staff to work from home in 2020, MSU was tasked with generating metadata projects suitable for library staff to work on remotely to assist with metadata quality efforts
- One such project was to request assistance from other NYPL divisions to find [URIs](/metadata-documentation/resources/glossary/#uniform-resource-identifier) for [Name Elements](/metadata-documentation/metadata/element/name/) and [Name Subject Elements](/metadata-documentation/metadata/element/subject/#name) where no URI was present
- At the start of the project, \~266,000 items had at least one Name Element without a URI and \~101,000 items had at least one Name Subject element without a URI
- Initial project collaborators were Access Services, SASB Periodicals Section, and General Humanities Operations with Preservation of Audio and Moving Image joining at a later date
- Since August 2021, the project has been fully taken over by MSU staff
- All applicable URIs have been found and batch updated in MMS for Name Elements previously without URIs
- Only a handful of divisions remain that are pending the identification and batch update of URIs for Name Subjects

---

Last updated September 2023
{: .float-right .fs-2 .text-grey-dk-000 }
### Friedman-Abeles Project: Legacy Digitization Title Updates & Name Subject Adds 

| Dates | beginning June 2020 |
| Collaborators | Billy Rose Theatre Division (Jeremy M., Steve M., Charlie M. and Brendan L.) with assistance from Tom L. and [PAMI](/metadata-documentation/resources/glossary/#preservation-of-audio-moving-image) staff |
| Related Links | [Google Slides for initial spreadsheet-based workflow 🔒](https://docs.google.com/presentation/d/1UDADAW9HOoMznR59MNf_-vwHWcMYpwJEjri6lf4SgrA/edit){: .btn } [JupyterLab notebook for current programmatic workflow 🔒](https://github.com/NYPL/metadata-projects/blob/main/in-progress/2020-06_friedman-abeles-titles-subjects/friedman-abeles_titles-subjects.ipynb){: .btn } [Friedman-Abeles photographs: [legacy collection] on Digital Collections](https://digitalcollections.nypl.org/collections/7a830280-c542-012f-b87c-58d385a7bc34){: .btn } |

#### Overview
{: .no_toc }

- When photographs from the Friedman-Abeles collection were originally digitized, the name of the production was automatically used as the item record titles, resulting in non-unique, duplicative, and non-descriptive titles
- When COVID-19 required staff to work remotely in March 2020, the Billy Rose Theatre Division staff began to prepare more descriptive titles with assistance from other departments
- Beginning in June 2020, MSU started its collaboration with the Theatre Division to programmatically batch update MMS records with these new titles
- Beginning August 2020, MSU also started adding [Name Subjects](/metadata-documentation/metadata/element/subject/#name) to records based on the names present in the new titles
- As a result of incorporating Name Subject additions to the project workflow, MSU created an internal "name thesaurus" to both organize name authority research and assist with batch programmatic updates
- As of September 2023, over 20,000 titles have been updated and 36,000 name subjects have been added

{: .note }
While the Library only holds one archival collection of [Friedman-Abeles photographs](https://archives.nypl.org/the/22538), there are currently two Friedman-Abeles photographs collections on Digital Collections. [Friedman-Abeles photographs: [legacy collection]](https://digitalcollections.nypl.org/collections/7a830280-c542-012f-b87c-58d385a7bc34) primarily consists of black and white photographs from the initial digitization project and is the current collection where Title Updates and Name Subject additions are being conducted. [Friedman-Abeles photographs](https://digitalcollections.nypl.org/collections/d3802d10-f49a-0139-3bff-0242ac110002) primarily consist of color photographs from the current digitization project and reflect the newly updated finding aid structure as of 2022. Once the mapping of the structure between the legacy and new collections is prepared, the digitized material in the legacy collection will be relocated to the new collection.

---

## Ongoing

---

Last updated September 2023
{: .float-right .fs-2 .text-grey-dk-000 }
### NYPL Wikidata Working Group

| Dates | beginning June 2023 |
| Collaborators | Bob K. (Music Division), David L. (Photography Collection) |
| Related Links | [WikiProject](https://www.wikidata.org/wiki/Wikidata:WikiProject_New_York_Public_Library){: .btn } [Google Group 🔒](https://groups.google.com/a/nypl.org/g/wikidata){: .btn } [Slack 🔒](https://nyplpscp.slack.com/archives/C05C3EMCBL7){: .btn } |

#### Overview
{: .no_toc }

- MSU leads the NYPL Wikidata Working Group, which began meeting monthly in July 2023
- The group's current focus is to establish and document best practices for the use of Wikidata to link to Library collections and resources on the [Wikidata:WikiProject New York Public Library page](https://www.wikidata.org/wiki/Wikidata:WikiProject_New_York_Public_Library)
- The group plans to open up to anyone interested in Wikidata at the Library in the future
- In the meantime, any Library staff members are welcome to join the #wikidata channel in the [Preservation and Collections Processing Slack 🔒](https://nyplpscp.slack.com/archives/C05C3EMCBL7) for updates and discussion;  [contact us](/metadata-documentation/contact/) for an invitation

---

Last updated September 2023
{: .float-right .fs-2 .text-grey-dk-000 }
### DEIA in Collections: Collections Access Working Group

| Dates | beginning February 2023 |
| Collaborators | see [Lair 🔒](https://lair.nypl.org/-/departments/internal-affairs/human-resources/diversity-equity-inclusion-access-at-nypl/deia-in-collections#:~:text=assess%20new%20acquisitions.-,Collections%20Access,-Chairs%3A%20Barrye%20Brown) |
| Related Links | [Lair 🔒](https://lair.nypl.org/-/departments/internal-affairs/human-resources/diversity-equity-inclusion-access-at-nypl/deia-in-collections#:~:text=assess%20new%20acquisitions.-,Collections%20Access,-Chairs%3A%20Barrye%20Brown){: .btn } |

#### Overview
{: .no_toc }

- The Manager, Metadata Services, is a member of the [Collections Access Working Group](https://lair.nypl.org/-/departments/internal-affairs/human-resources/diversity-equity-inclusion-access-at-nypl/deia-in-collections#:~:text=assess%20new%20acquisitions.-,Collections%20Access,-Chairs%3A%20Barrye%20Brown), which evolved out of the DEIA in Collections working group initiated in 2021
- The group is working to incorporate the principles of DEIA collecting into the ways our holdings are digitized and deployed
- Building on the work of projects like Change the Subject, staff will interrogate the history and legacy of descriptive practices and recommend changes for the future, while also reviewing our ongoing digitization efforts that focus on DEIA work and how we promote the collections we have described and digitized through reference resources and outreach like LibGuides and blogs

---

Last updated September 2023
{: .float-right .fs-2 .text-grey-dk-000 }
### Links to NYPL Digital Collections from Catalog

| Dates | beginning December 2021 (initial refresh occurred between January–September 2022) |
| Collaborators | ILS Team (Aaron D., Antonio S.); Special Collections Processing; BookOps |
| Related Links | [metadata-tools 🔒](https://github.com/NYPL/metadata-projects/tree/main/ongoing/bnumber-links-to-dc){: .btn } [Data Supplied to ILS Team 🔒](https://drive.google.com/drive/folders/1ktPZqRYoIv0yJIWTwLDeRhM766GKaDU7?usp=sharing){: .btn } [MMS › Workflows / Linking Between Systems / Research Catalog](/metadata-documentation/workflows/linking/#research-catalog){: .btn } [MMS › Metadata / By Element / Identifier / NYPL catalog ID (B-number)](/metadata-documentation/metadata/element/identifier/bnumber/){: .btn } |

#### Overview
{: .no_toc }

- MSU developed a new workflow with the ILS Team to systematically add and maintain links from the [Library catalog](https://www.nypl.org/research/research-catalog/) to corresponding digitized materials
- Prior to this project, the catalog contained 17,525 records with links to NYPL Digital Collections (DC)
- An additional 6,340 records featured broken links, including links to predecessors to DC such as Digital Gallery
- Through a combination of newly automated processes and manual review of discrepancies, MSU was able to nearly double the number of records in the catalog that displayed active links to DC to 33,401 records with our initial refresh in September 2022
- MSU was also able to improve the quantity and quality of links from DC to the catalog and standardize previously-inconsistent link labels as they appear in the library catalog
- MSU is continuing to refine our workflow with the goal of supplying refreshed data to the Library's ILS Team on a regular basis so they can perform batch updates
- By increasing access between the two systems, this effort contributes to an improved patron experience for users of both the catalog and NYPL Digital Collections

---

Last updated November 2023
{: .float-right .fs-2 .text-grey-dk-000 }
### Systematic Library of Congress Subject Element Updates

| Dates | beginning May 2023 |
| Related Links | [By Element › Subject](/metadata-documentation/metadata/element/subject/); [Library of Congress' Bulk Export of Library of Congress Subject Headings](https://id.loc.gov/authorities/subjects.html#:~:text=SKOS%20%2D%20JSON-,Bulk%20Download,-Bulk%20exports%20%2D%20MADS); [Controlled Vocabularies](/metadata-documentation/metadata/guidelines/#controlled-vocabularies) |

#### Overview
{: .no_toc }

- Many [Subject](/metadata-documentation/metadata/element/subject/) element terms in MMS records do not match terms in MSU's preferred [controlled vocabularies](/metadata-documentation/metadata/guidelines/#controlled-vocabularies)
- These discrepancies occur when outdated terms are used in source records [imported into MMS](/metadata-documentation/workflows/importing/), when terms are updated in the controlled vocabulary after metadata import, and when terms are selected using the MMS authorities module, which is only periodically updated and therefore may be out of sync with the respective source vocabulary
- To address these outdated terms, MSU is developing a workflow to systematically and programmatically update [Subject](/metadata-documentation/metadata/element/subject/) elements in MMS records on a regular basis, starting with LCSH terms using the [Library of Congress Bulk Export of Library of Congress Subject Headings](https://id.loc.gov/authorities/subjects.html#:~:text=SKOS%20%2D%20JSON-,Bulk%20Download,-Bulk%20exports%20%2D%20MADS)
- This project was initiated following the March 2023 Library of Congress revision of the term "Slaves" to "[Enslaved persons](http://id.loc.gov/authorities/subjects/sh85123347)," which prompted MSU to update [this term and other related terms](https://docs.google.com/spreadsheets/d/1OqTynL9Y5fe8o6VfmCh9MKR97zsF0Kr-FLvfdvD9LlI/edit#gid=1491352248), affecting 873 approved records and 763 draft records in MMS

---

Last updated September 2023
{: .float-right .fs-2 .text-grey-dk-000 }
### Inclusive & Reparative Description

| Dates | beginning April 2022 |
| Collaborators | DEIA in Collections: Collections Access Working Group; Digital Collections Services; Curatorial Divisions |
| Related Links | [General Guidelines › Inclusive & Reparative Description](/metadata-documentation/metadata/inclusive-reparative/); [NYPL's Statement on Potentially Harmful Content](https://digitalcollections.nypl.org/about#nypl_harmful_content_statement) |

#### Overview
{: .no_toc }

- MSU is committed to integrating inclusive and reparative description into our everyday work and has led several efforts to address harmful description and content on NYPL Digital Collections
- Informed by MSU staff's participation in professional development and the Library’s [DEIA in Collections: Collections Access Working Group](#deia-in-collections-collections-access-working-group), MSU maintains internal guidelines and workflows, which can be found at [MMS › Metadata › Inclusive & Reparative Description](/metadata-documentation/metadata/inclusive-reparative/)
- MSU is developing ideas for specific holistic remediation projects to align extant legacy description with updated guidelines
- Inclusive and reparative description efforts will continue to evolve based on feedback from Library staff and patrons; please [contact us](/metadata-documentation/contact/form/) if you have ideas, concerns, or questions related to NYPL Digital Collections content and description

---

## Completed

---

Last updated September 2023
{: .float-right .fs-2 .text-grey-dk-000 }
### Michael Cummings African American Art Event Ephemera Collection on Wikidata

| Dates | December 2022–January 2023 |
| Collaborators | Schomburg Art & Artifacts; Kimberly H. (Schomburg); participants of the December 2022 Wiki Edu Wikidata Office Hours Course |
| Related Links | [WikiProject](https://www.wikidata.org/wiki/Wikidata:WikiProject_New_York_Public_Library/Projects#Michael_Cummings_African_American_Art_Event_Ephemera_Collection){: .btn } [Michael Cummings & A Bygone Era in Art](https://www.nypl.org/events/exhibitions/michael-cummings-bygone-era-art){: .btn } [Google Sheet 🔒](https://docs.google.com/spreadsheets/d/1lrgiZmo7PL-wCgF5hb4qzf8UNRC2h0erBRy8pV6tvd8/edit){: .btn } [GitHub 🔒](https://github.com/NYPL/metadata-projects/tree/main/x_completed/2023-05_michael-cummings-art-event-ephemera){: .btn } |


#### Overview
{: .no_toc }

- MSU led a project to enhance Wikidata with information derived from a [digitized portion](https://digitalcollections.nypl.org/collections/7d10f150-e9c8-013a-8b28-0242ac110003) of the [Michael Cummings African American Art Event Ephemera Collection](https://legacycatalog.nypl.org/record=b22808222~S1), which consists of posters, pamphlets, postcard, fliers, brochures, and other print material used to advertise or announce art exhibitions and events related to work created by Black and Latinx artists.
- In total, [over 500 Wikidata items](https://pagepile.toolforge.org/api.php?id=50203\&action=get_data\&format=html) were part of the project—including items for 350+ people (artists, curators, etc.), 40+ galleries/museums, and 70+ exhibitions
- Of these, MSU created 290 new Wikidata items for entities such as [Cayman Gallery](https://www.wikidata.org/wiki/Q115626588), [Oakley N. Holmes, Jr.](https://www.wikidata.org/wiki/Q115621470), [Lillian Blades](https://www.wikidata.org/wiki/Q115626488), [_Harlem Artists 69_](https://www.wikidata.org/wiki/Q115688926), and many others
- Additionally, MSU enhanced Wikidata items with [references](https://query.wikidata.org/embed.html#SELECT%20%3Fstatement%20%3Fsubject%20%3FsubjectLabel%20%3Fproperty%20%3FpropertyLabel%20%3Fobject%20%3FobjectLabel%20%3FrefURL%20WITH%0A%7B%0A%20%20SELECT%20DISTINCT%20%3Fsubject%20WHERE%20%7B%0A%20%20%20%20%7B%0A%20%20%20%20%20%20SERVICE%20wikibase%3Amwapi%20%7B%0A%20%20%20%20%20%20%20%20bd%3AserviceParam%20wikibase%3Aendpoint%20%22www.wikidata.org%22%3B%20wikibase%3Aapi%20%22Generator%22%3B%20mwapi%3Agenerator%20%22exturlusage%22%3B%20mwapi%3Ageulimit%20%22500%22%3B%20mwapi%3Ageuquery%20%22digitalcollections.nypl.org%22%3B%20mwapi%3Ageuprotocol%20%22http%22%3B%20mwapi%3Ageunamespace%20%220%22%20.%0A%20%20%20%20%20%20%20%20%3Ftitle%20wikibase%3AapiOutput%20mwapi%3Atitle.%0A%20%20%20%20%20%20%7D%0A%20%20%20%20%7D%20UNION%20%7B%0A%20%20%20%20%20%20SERVICE%20wikibase%3Amwapi%20%7B%0A%20%20%20%20%20%20%20%20bd%3AserviceParam%20wikibase%3Aendpoint%20%22www.wikidata.org%22%3B%20wikibase%3Aapi%20%22Generator%22%3B%20mwapi%3Agenerator%20%22exturlusage%22%3B%20mwapi%3Ageulimit%20%22500%22%3B%20mwapi%3Ageuquery%20%22digitalcollections.nypl.org%22%3B%20mwapi%3Ageuprotocol%20%22https%22%3B%20mwapi%3Ageunamespace%20%220%22%20.%0A%20%20%20%20%20%20%20%20%3Ftitle%20wikibase%3AapiOutput%20mwapi%3Atitle.%0A%20%20%20%20%20%20%7D%0A%20%20%20%20%7D%0A%20%20%20%20BIND%28IRI%28CONCAT%28STR%28wd%3A%29%2C%20%3Ftitle%29%29%20AS%20%3Fsubject%29%0A%20%20%7D%0A%7D%20AS%20%25items%20%7B%0A%20%20INCLUDE%20%25items%20.%0A%20%20%0A%20%20hint%3AQuery%20hint%3Aoptimizer%20%22None%22.%0A%20%20%0A%20%20%3Fsubject%20%3Fp%20%3Fstatement%20.%0A%20%20%3Fstatement%20prov%3AwasDerivedFrom%2Fpr%3AP854%20%3FrefURL%20.%0A%20%20FILTER%20%28CONTAINS%28str%28%3FrefURL%29%2C%20%27digitalcollections.nypl.org%2F%27%29%29%20.%0A%0A%20%20FILTER%20%28%3Fsubject%20IN%20%28wd%3AQ115688683%2C%20wd%3AQ116025448%2C%20wd%3AQ115688872%2C%20wd%3AQ115690302%2C%20wd%3AQ115707713%2C%20wd%3AQ115707790%2C%20wd%3AQ115688843%2C%20wd%3AQ116025383%2C%20wd%3AQ4647184%2C%20wd%3AQ4661979%2C%20wd%3AQ115651716%2C%20wd%3AQ115620805%2C%20wd%3AQ93361249%2C%20wd%3AQ116025124%2C%20wd%3AQ116018261%2C%20wd%3AQ28871314%2C%20wd%3AQ115620809%2C%20wd%3AQ115620814%2C%20wd%3AQ115830223%2C%20wd%3AQ4689456%2C%20wd%3AQ379613%2C%20wd%3AQ4738121%2C%20wd%3AQ4738077%2C%20wd%3AQ115626964%2C%20wd%3AQ24055555%2C%20wd%3AQ115651077%2C%20wd%3AQ114917008%2C%20wd%3AQ4725999%2C%20wd%3AQ4727179%2C%20wd%3AQ28861370%2C%20wd%3AQ17305826%2C%20wd%3AQ4738121%2C%20wd%3AQ6940773%2C%20wd%3AQ354783%2C%20wd%3AQ115701826%2C%20wd%3AQ115690772%2C%20wd%3AQ27734639%2C%20wd%3AQ28861359%2C%20wd%3AQ115682467%2C%20wd%3AQ115626543%2C%20wd%3AQ115620916%2C%20wd%3AQ94279830%2C%20wd%3AQ18416765%2C%20wd%3AQ115688730%2C%20wd%3AQ21136215%2C%20wd%3AQ115690583%2C%20wd%3AQ27055887%2C%20wd%3AQ115626550%2C%20wd%3AQ22129708%2C%20wd%3AQ2883927%2C%20wd%3AQ115651078%2C%20wd%3AQ5339271%2C%20wd%3AQ4885382%2C%20wd%3AQ115651080%2C%20wd%3AQ28858711%2C%20wd%3AQ28914109%2C%20wd%3AQ4889934%2C%20wd%3AQ12887972%2C%20wd%3AQ37892461%2C%20wd%3AQ115651082%2C%20wd%3AQ4898721%2C%20wd%3AQ2900288%2C%20wd%3AQ28858501%2C%20wd%3AQ718617%2C%20wd%3AQ116025159%2C%20wd%3AQ115690627%2C%20wd%3AQ115700509%2C%20wd%3AQ115700522%2C%20wd%3AQ115700519%2C%20wd%3AQ115700521%2C%20wd%3AQ115700520%2C%20wd%3AQ115626563%2C%20wd%3AQ115690563%2C%20wd%3AQ65937145%2C%20wd%3AQ115690884%2C%20wd%3AQ109954129%2C%20wd%3AQ115700089%2C%20wd%3AQ5026623%2C%20wd%3AQ115626577%2C%20wd%3AQ28871563%2C%20wd%3AQ115621138%2C%20wd%3AQ115626953%2C%20wd%3AQ28860566%2C%20wd%3AQ28858316%2C%20wd%3AQ16121853%2C%20wd%3AQ105839708%2C%20wd%3AQ115702545%2C%20wd%3AQ28913883%2C%20wd%3AQ115626588%2C%20wd%3AQ115701853%2C%20wd%3AQ115651084%2C%20wd%3AQ1906150%2C%20wd%3AQ28860562%2C%20wd%3AQ115621111%2C%20wd%3AQ21751027%2C%20wd%3AQ5083521%2C%20wd%3AQ23542711%2C%20wd%3AQ115651086%2C%20wd%3AQ115651088%2C%20wd%3AQ111337590%2C%20wd%3AQ115651090%2C%20wd%3AQ115621240%2C%20wd%3AQ28860251%2C%20wd%3AQ103849821%2C%20wd%3AQ115651091%2C%20wd%3AQ115626619%2C%20wd%3AQ115621265%2C%20wd%3AQ115689522%2C%20wd%3AQ115700448%2C%20wd%3AQ115707735%2C%20wd%3AQ115651093%2C%20wd%3AQ115650882%2C%20wd%3AQ115650869%2C%20wd%3AQ116025305%2C%20wd%3AQ115689403%2C%20wd%3AQ5170231%2C%20wd%3AQ115770098%2C%20wd%3AQ18685644%2C%20wd%3AQ28865181%2C%20wd%3AQ19661797%2C%20wd%3AQ115651095%2C%20wd%3AQ21486065%2C%20wd%3AQ5220829%2C%20wd%3AQ115650644%2C%20wd%3AQ115651097%2C%20wd%3AQ109646910%2C%20wd%3AQ5232007%2C%20wd%3AQ320846%2C%20wd%3AQ115651099%2C%20wd%3AQ28914215%2C%20wd%3AQ115621313%2C%20wd%3AQ5239003%2C%20wd%3AQ115621414%2C%20wd%3AQ115651100%2C%20wd%3AQ74067002%2C%20wd%3AQ115651131%2C%20wd%3AQ106307681%2C%20wd%3AQ115921935%2C%20wd%3AQ115651132%2C%20wd%3AQ13560695%2C%20wd%3AQ4547697%2C%20wd%3AQ115621409%2C%20wd%3AQ115621424%2C%20wd%3AQ115621470%2C%20wd%3AQ9075813%2C%20wd%3AQ115921562%2C%20wd%3AQ115707839%2C%20wd%3AQ115621519%2C%20wd%3AQ115621529%2C%20wd%3AQ94539793%2C%20wd%3AQ115621541%2C%20wd%3AQ115638838%2C%20wd%3AQ115651133%2C%20wd%3AQ115651101%2C%20wd%3AQ1264273%2C%20wd%3AQ5353662%2C%20wd%3AQ290331%2C%20wd%3AQ20810858%2C%20wd%3AQ5372719%2C%20wd%3AQ24049045%2C%20wd%3AQ115650615%2C%20wd%3AQ5392935%2C%20wd%3AQ115650588%2C%20wd%3AQ115650566%2C%20wd%3AQ5431220%2C%20wd%3AQ858689%2C%20wd%3AQ28755558%2C%20wd%3AQ115621532%2C%20wd%3AQ115651102%2C%20wd%3AQ115621817%2C%20wd%3AQ100250105%2C%20wd%3AQ1442122%2C%20wd%3AQ116025410%2C%20wd%3AQ18707510%2C%20wd%3AQ106620804%2C%20wd%3AQ78880465%2C%20wd%3AQ115702613%2C%20wd%3AQ3087143%2C%20wd%3AQ5504731%2C%20wd%3AQ115700373%2C%20wd%3AQ115626696%2C%20wd%3AQ115650542%2C%20wd%3AQ115639780%2C%20wd%3AQ115621813%2C%20wd%3AQ115651104%2C%20wd%3AQ115651105%2C%20wd%3AQ100235674%2C%20wd%3AQ115651107%2C%20wd%3AQ77353140%2C%20wd%3AQ84496231%2C%20wd%3AQ115648607%2C%20wd%3AQ5568294%2C%20wd%3AQ365682%2C%20wd%3AQ115700044%2C%20wd%3AQ106307830%2C%20wd%3AQ28871545%2C%20wd%3AQ42796033%2C%20wd%3AQ115650528%2C%20wd%3AQ115651108%2C%20wd%3AQ115690807%2C%20wd%3AQ115621808%2C%20wd%3AQ15489989%2C%20wd%3AQ115621807%2C%20wd%3AQ5645872%2C%20wd%3AQ20180409%2C%20wd%3AQ189074%2C%20wd%3AQ115688926%2C%20wd%3AQ116025468%2C%20wd%3AQ115650448%2C%20wd%3AQ115626395%2C%20wd%3AQ114751406%2C%20wd%3AQ5728819%2C%20wd%3AQ115707746%2C%20wd%3AQ5864249%2C%20wd%3AQ72853273%2C%20wd%3AQ10966148%2C%20wd%3AQ1396266%2C%20wd%3AQ115651109%2C%20wd%3AQ115651111%2C%20wd%3AQ18685493%2C%20wd%3AQ116025138%2C%20wd%3AQ1631871%2C%20wd%3AQ11863692%2C%20wd%3AQ77589010%2C%20wd%3AQ5921354%2C%20wd%3AQ115922559%2C%20wd%3AQ115626375%2C%20wd%3AQ5933571%2C%20wd%3AQ115626373%2C%20wd%3AQ115829542%2C%20wd%3AQ115701986%2C%20wd%3AQ115701792%2C%20wd%3AQ115688761%2C%20wd%3AQ115829216%2C%20wd%3AQ116025268%2C%20wd%3AQ6049440%2C%20wd%3AQ115921901%2C%20wd%3AQ115921713%2C%20wd%3AQ115922541%2C%20wd%3AQ115921701%2C%20wd%3AQ115626371%2C%20wd%3AQ76225882%2C%20wd%3AQ115650312%2C%20wd%3AQ6217391%2C%20wd%3AQ6115781%2C%20wd%3AQ355566%2C%20wd%3AQ115651112%2C%20wd%3AQ6127277%2C%20wd%3AQ115626360%2C%20wd%3AQ115626352%2C%20wd%3AQ115651113%2C%20wd%3AQ115651114%2C%20wd%3AQ28869312%2C%20wd%3AQ115700485%2C%20wd%3AQ21857909%2C%20wd%3AQ95479576%2C%20wd%3AQ109648740%2C%20wd%3AQ21994092%2C%20wd%3AQ28914213%2C%20wd%3AQ107140668%2C%20wd%3AQ112208957%2C%20wd%3AQ115651115%2C%20wd%3AQ115650341%2C%20wd%3AQ115626628%2C%20wd%3AQ115651117%2C%20wd%3AQ115651118%2C%20wd%3AQ28366284%2C%20wd%3AQ55219739%2C%20wd%3AQ115651119%2C%20wd%3AQ115626408%2C%20wd%3AQ115626406%2C%20wd%3AQ21849415%2C%20wd%3AQ115651120%2C%20wd%3AQ115651121%2C%20wd%3AQ6251417%2C%20wd%3AQ115648628%2C%20wd%3AQ65073550%2C%20wd%3AQ6260101%2C%20wd%3AQ15516987%2C%20wd%3AQ6260101%2C%20wd%3AQ115626401%2C%20wd%3AQ6282568%2C%20wd%3AQ115822656%2C%20wd%3AQ115626399%2C%20wd%3AQ115651802%2C%20wd%3AQ55566681%2C%20wd%3AQ115626415%2C%20wd%3AQ115626414%2C%20wd%3AQ115626413%2C%20wd%3AQ28860548%2C%20wd%3AQ112201286%2C%20wd%3AQ23014998%2C%20wd%3AQ55563173%2C%20wd%3AQ115651122%2C%20wd%3AQ115651123%2C%20wd%3AQ115626412%2C%20wd%3AQ28173191%2C%20wd%3AQ28871214%2C%20wd%3AQ108755841%2C%20wd%3AQ3210324%2C%20wd%3AQ3210324%2C%20wd%3AQ115626459%2C%20wd%3AQ6490865%2C%20wd%3AQ115648648%2C%20wd%3AQ6509419%2C%20wd%3AQ115626474%2C%20wd%3AQ115689431%2C%20wd%3AQ115650489%2C%20wd%3AQ23682750%2C%20wd%3AQ562912%2C%20wd%3AQ115651124%2C%20wd%3AQ1821821%2C%20wd%3AQ115650720%2C%20wd%3AQ115626488%2C%20wd%3AQ115650751%2C%20wd%3AQ28735382%2C%20wd%3AQ115651125%2C%20wd%3AQ28871085%2C%20wd%3AQ100235717%2C%20wd%3AQ3258676%2C%20wd%3AQ115689045%2C%20wd%3AQ28542256%2C%20wd%3AQ3709122%2C%20wd%3AQ97015284%2C%20wd%3AQ797599%2C%20wd%3AQ115650798%2C%20wd%3AQ115626496%2C%20wd%3AQ28871580%2C%20wd%3AQ115651126%2C%20wd%3AQ115651127%2C%20wd%3AQ16115301%2C%20wd%3AQ19757494%2C%20wd%3AQ50104300%2C%20wd%3AQ1367166%2C%20wd%3AQ109647054%2C%20wd%3AQ100235687%2C%20wd%3AQ115626515%2C%20wd%3AQ6776418%2C%20wd%3AQ115650823%2C%20wd%3AQ28943185%2C%20wd%3AQ3305305%2C%20wd%3AQ115731752%2C%20wd%3AQ115702669%2C%20wd%3AQ115701888%2C%20wd%3AQ6820728%2C%20wd%3AQ115650858%2C%20wd%3AQ17017286%2C%20wd%3AQ115651129%2C%20wd%3AQ115707704%2C%20wd%3AQ100235671%2C%20wd%3AQ2684150%2C%20wd%3AQ28855057%2C%20wd%3AQ115650927%2C%20wd%3AQ100240572%2C%20wd%3AQ115690280%2C%20wd%3AQ115650850%2C%20wd%3AQ115626524%2C%20wd%3AQ4274641%2C%20wd%3AQ115702633%2C%20wd%3AQ115650940%2C%20wd%3AQ28860582%2C%20wd%3AQ6971006%2C%20wd%3AQ6971006%2C%20wd%3AQ777636%2C%20wd%3AQ115648132%2C%20wd%3AQ115824849%2C%20wd%3AQ116018541%2C%20wd%3AQ115626522%2C%20wd%3AQ115626519%2C%20wd%3AQ115651135%2C%20wd%3AQ28871617%2C%20wd%3AQ115921545%2C%20wd%3AQ115651136%2C%20wd%3AQ21995261%2C%20wd%3AQ16016249%2C%20wd%3AQ7052490%2C%20wd%3AQ115626516%2C%20wd%3AQ115700067%2C%20wd%3AQ115621793%2C%20wd%3AQ115651237%2C%20wd%3AQ115621789%2C%20wd%3AQ87299557%2C%20wd%3AQ22279380%2C%20wd%3AQ115702675%2C%20wd%3AQ115700043%2C%20wd%3AQ3361615%2C%20wd%3AQ115707812%2C%20wd%3AQ28865210%2C%20wd%3AQ115621770%2C%20wd%3AQ7149748%2C%20wd%3AQ115648069%2C%20wd%3AQ115651137%2C%20wd%3AQ100240037%2C%20wd%3AQ115690745%2C%20wd%3AQ115690976%2C%20wd%3AQ556585%2C%20wd%3AQ22275399%2C%20wd%3AQ115633678%2C%20wd%3AQ115651139%2C%20wd%3AQ115828833%2C%20wd%3AQ115690822%2C%20wd%3AQ115700498%2C%20wd%3AQ115621762%2C%20wd%3AQ115770410%2C%20wd%3AQ115621764%2C%20wd%3AQ115633675%2C%20wd%3AQ115621765%2C%20wd%3AQ7326615%2C%20wd%3AQ94542171%2C%20wd%3AQ19605041%2C%20wd%3AQ115621767%2C%20wd%3AQ115633661%2C%20wd%3AQ115621730%2C%20wd%3AQ115621761%2C%20wd%3AQ115651254%2C%20wd%3AQ28870365%2C%20wd%3AQ115633237%2C%20wd%3AQ107410750%2C%20wd%3AQ115651140%2C%20wd%3AQ115621736%2C%20wd%3AQ16104439%2C%20wd%3AQ1291679%2C%20wd%3AQ26899613%2C%20wd%3AQ115651141%2C%20wd%3AQ115621758%2C%20wd%3AQ7373054%2C%20wd%3AQ115633229%2C%20wd%3AQ115633215%2C%20wd%3AQ115626919%2C%20wd%3AQ116033464%2C%20wd%3AQ18645873%2C%20wd%3AQ2216478%2C%20wd%3AQ7409275%2C%20wd%3AQ28871394%2C%20wd%3AQ115707764%2C%20wd%3AQ115822535%2C%20wd%3AQ115651142%2C%20wd%3AQ115621749%2C%20wd%3AQ115633206%2C%20wd%3AQ115651143%2C%20wd%3AQ107689883%2C%20wd%3AQ1060566%2C%20wd%3AQ100250031%2C%20wd%3AQ115689561%2C%20wd%3AQ115700471%2C%20wd%3AQ115690607%2C%20wd%3AQ115921578%2C%20wd%3AQ115770274%2C%20wd%3AQ115701947%2C%20wd%3AQ116025381%2C%20wd%3AQ16106761%2C%20wd%3AQ7491043%2C%20wd%3AQ42156278%2C%20wd%3AQ115621680%2C%20wd%3AQ115621685%2C%20wd%3AQ115633188%2C%20wd%3AQ115690285%2C%20wd%3AQ1192305%2C%20wd%3AQ7554744%2C%20wd%3AQ115690314%2C%20wd%3AQ1601838%2C%20wd%3AQ115702288%2C%20wd%3AQ99797229%2C%20wd%3AQ115626915%2C%20wd%3AQ28861822%2C%20wd%3AQ106518731%2C%20wd%3AQ115621705%2C%20wd%3AQ115651301%2C%20wd%3AQ28223041%2C%20wd%3AQ115621713%2C%20wd%3AQ115770320%2C%20wd%3AQ115621714%2C%20wd%3AQ7704039%2C%20wd%3AQ100235703%2C%20wd%3AQ7707677%2C%20wd%3AQ72854644%2C%20wd%3AQ115690878%2C%20wd%3AQ4974195%2C%20wd%3AQ632682%2C%20wd%3AQ5020212%2C%20wd%3AQ27330476%2C%20wd%3AQ115626735%2C%20wd%3AQ115689466%2C%20wd%3AQ116025273%2C%20wd%3AQ77589010%2C%20wd%3AQ115651332%2C%20wd%3AQ4328346%2C%20wd%3AQ903403%2C%20wd%3AQ115702664%2C%20wd%3AQ116025390%2C%20wd%3AQ115633143%2C%20wd%3AQ7793969%2C%20wd%3AQ89886924%2C%20wd%3AQ115650906%2C%20wd%3AQ102102133%2C%20wd%3AQ102102133%2C%20wd%3AQ7815762%2C%20wd%3AQ114924038%2C%20wd%3AQ50345522%2C%20wd%3AQ115690819%2C%20wd%3AQ28871717%2C%20wd%3AQ115689409%2C%20wd%3AQ115689465%2C%20wd%3AQ115626716%2C%20wd%3AQ115626725%2C%20wd%3AQ115626729%2C%20wd%3AQ115770467%2C%20wd%3AQ115633128%2C%20wd%3AQ7911308%2C%20wd%3AQ115691026%2C%20wd%3AQ19849610%2C%20wd%3AQ21293102%2C%20wd%3AQ115621653%2C%20wd%3AQ20715407%2C%20wd%3AQ115707825%2C%20wd%3AQ60735862%2C%20wd%3AQ100240076%2C%20wd%3AQ28914195%2C%20wd%3AQ115633116%2C%20wd%3AQ115702142%2C%20wd%3AQ24204395%2C%20wd%3AQ7996460%2C%20wd%3AQ115689572%2C%20wd%3AQ115621636%2C%20wd%3AQ115621594%2C%20wd%3AQ115621599%2C%20wd%3AQ115651144%2C%20wd%3AQ8010139%2C%20wd%3AQ1883000%2C%20wd%3AQ115651146%2C%20wd%3AQ115621611%2C%20wd%3AQ19573553%2C%20wd%3AQ115651184%2C%20wd%3AQ8019143%2C%20wd%3AQ115700435%2C%20wd%3AQ115690967%2C%20wd%3AQ8032772%2C%20wd%3AQ115691085%2C%20wd%3AQ8043522%29%29.%0A%20%20%0A%20%20%3Fproperty%20wikibase%3Aclaim%20%3Fp%20.%0A%20%20%3Fproperty%20wikibase%3AstatementProperty%20%3Fps%20.%0A%20%20%3Fstatement%20%3Fps%20%3Fobject%20.%0A%20%20%0A%20%20SERVICE%20wikibase%3Alabel%20%7B%20bd%3AserviceParam%20wikibase%3Alanguage%20%22en%22%20%7D%0A%7D%0AORDER%20BY%20ASC%28%3FsubjectLabel%29) to the relevant material in [NYPL Digital Collections](https://digitalcollections.nypl.org/collections/7d10f150-e9c8-013a-8b28-0242ac110003) and experimented with new methods to reuse data from Wikidata in the Metadata Management System (MMS)
- Related SPARQL queries can be found on the the Library's [WikiProject](https://www.wikidata.org/wiki/Wikidata:WikiProject_New_York_Public_Library/Projects#Michael_Cummings_African_American_Art_Event_Ephemera_Collection)