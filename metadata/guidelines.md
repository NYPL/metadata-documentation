---
layout: page
title: General Guidelines
permalink: /metadata/guidelines/
parent: MMS › Metadata
nav_order: 2
---

# General Guidelines
{: .no_toc }

Provides broader guidance on standards and best practices for metadata in the context of the Metadata Management System (MMS)

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Metadata Schema
- ​​A metadata schema outlines the overall structure for a record
- Records in MMS are structured using the [Metadata Object Description Schema (MODS)](/metadata-documentation/resources/glossary/#metadata-object-description-schema)
- MMS uses selections from MODS elements up to [version 3.4](https://www.loc.gov/standards/mods/mods-3-4-announcement.html)
- Our local guidelines for MODS elements, subelements, and attributes can be found in the [MMS › Metadata / By Element](/metadata-documentation/metadata/element/) section of this site
    - Look for the **View MODS Documentation →** links throughout our documentation to view the corresponding documentation from the Library of Congress

## Content Standards
- A metadata content standard describes guidelines for the format and syntax of the data values that are used to populate metadata elements
- Format and syntax of metadata elements should be governed by the relevant content standard
    - For bibliographic materials, refer to [Resource Description & Access (RDA)](/metadata-documentation/resources/glossary/#resource-description-and-access)
    - For archival materials, refer to [Describing Archives: A Content Standard (DACS)](/metadata-documentation/resources/glossary/#describing-archives-a-content-standard)
    - See [NYPL Documentation](/metadata-documentation/resources/external/#nypl-documentation) for links to documentation produced by other departments of the Library, which provide additional guidelines on format and syntax

## Controlled Vocabularies
- A controlled vocabulary is a list of terms, names, or other standardized values that can be used to populate metadata elements and subelements in a consistent manner that supports searching and browsing
- Authority control is the process of selecting from a controlled vocabulary, which may also be referred to interchangeably as an authority or thesaurus
- In MMS, [Name](/metadata-documentation/metadata/element/name/), [Genre](/metadata-documentation/metadata/element/genre/), and [Subject](/metadata-documentation/metadata/element/subject/) elements, and the [Form](/metadata-documentation/metadata/element/physical-description/#form) subelement include a lookup feature to search controlled vocabularies, internally referenced as the MMS authorities module
  - The MMS authorities module is accessed by clicking the **Authority data search** link within a controlled element or subelement, where you can search authorized terms from:
    - [Library of Congress Linked Data Service](https://id.loc.gov/)
      - [Library of Congress Subject Headings (LCSH)](https://id.loc.gov/authorities/subjects.html)
      - [Library of Congress Name Authority File (LCNAF)](https://id.loc.gov/authorities/names.html)
      - [Library of Congress Genre/Form Terms (LCGFT)](https://id.loc.gov/authorities/genreForms.html)
      - [Thesaurus for Graphic Materials (TGM)](https://id.loc.gov/vocabulary/graphicMaterials.html)
    - [Getty Art & Architecture Thesaurus (AAT)](https://www.getty.edu/research/tools/vocabularies/aat/)
  - Data displayed by the MMS authorities module is only periodically updated and therefore may be out of sync with the respective source vocabulary
- While the MMS authorities module does not support searching the [Virtual International Authority File (VIAF)](http://viaf.org/), names found in VIAF can be added manually for the [Name](/metadata-documentation/metadata/element/name/#name-part) element and [Name Subject](/metadata-documentation/metadata/element/subject/#name) subelement
- Consult the respective [element](/metadata-documentation/metadata/element/) guidelines for an explanation of which vocabularies are displayed and preferred for a particular element or subelement, as well as when it is appropriate (and how) to add terms or names manually

## Inheritance
- The inheritance functionality within MMS facilitates efficient metadata creation by eliminating repetitive re-keying of data
- Inheritance should be carefully considered when used
- All [elements](/metadata-documentation/metadata/element/) in the **Descriptive metadata** tab of a collection or container records have a corresponding **Inheritable** checkbox
- Inherited metadata elements can be found in the **Descriptive metadata** tab of a container or item record under **Inherited elements**
    - Elements in gray are inherited from another record
    - Yellow highlighted elements are inheritable from a given record
    - Click the **Override** link in the **Inherited elements** section to disinherit a metadata element
        - If **Override** is clicked on a collection or container, the metadata element will also be disinherited from all records contained by that record

## Minimum Metadata Requirements
MMS item records must include the following seven descriptive metadata elements/subelements, either assigned or inherited, to be approved to appear on Digital Collections (see [Approvals](/metadata-documentation/workflows/approvals/))
1. [Title](/metadata-documentation/metadata/element/title/)
1. [Type of Resource](/metadata-documentation/metadata/element/type-of-resource/)
1. [Identifier](/metadata-documentation/metadata/element/identifier/)
1. [Date](/metadata-documentation/metadata/element/origin-info/#date) (sublement of [Origin Info](/metadata-documentation/metadata/element/origin-info/))
1. [Genre](/metadata-documentation/metadata/element/genre/)
1. [Location](/metadata-documentation/metadata/element/location/)
1. [Language](/metadata-documentation/metadata/element/language/) (if applicable)

## Rights
- Rights metadata determines:
    - Whether approved records [appear on Digital Collections](/metadata-documentation/dc/criteria/) based on **Approved use**:
        - **Can be used on NYPL website**: available globally
        - **Can be displayed on NYPL premises**: available from any computer connected to the internet at any Research or Branch location of the New York Public Library
        - **Can be displayed on NYPL premises :: location, LPA-wide**: available from any computer connected to the internet at the Library for the Performing Arts
    - Whether and how assets can be downloaded
- Rights information can be found on the **Overview** and **Rights and use** tabs of a record
    - The **Rights** section of the **Overview** tab indicates whether rights are set at that record's level or inherited as well as information about when rights were created or updated rights and by whom
    - The **Rights and use** tab displays what is shown on the **Overview** tab as well as **Approved uses** and a **Rights Research and Copyright Information Summary**
        - Codes used for the **Copyright status** in the **Rights Research and Copyright Information Summary** are defined on the [Rights Codes Cheat Sheet 🔒](https://confluence.nypl.org/x/BIBy)
- Rights are added and maintained by [Copyright and Information Policy](/metadata-documentation/resources/glossary/#copyright-information-policy)
- See [MMS › Workflows › Rights](/metadata-documentation/workflows/rights/) for the process when Metadata Services Unit (MSU) requests rights metadata be added to records in the Metadata Management System (MMS) by Copyright and Information Policy (CIP)