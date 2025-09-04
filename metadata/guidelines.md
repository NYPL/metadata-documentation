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
- Rights are added and maintained by [Rights Clearance](/metadata-documentation/resources/glossary/#rights-clearance)
  - See [MMS › Workflows › Rights](/metadata-documentation/workflows/rights/) for the process when MSU requests rights metadata be added to records in MMS by Rights Clearance
- Rights metadata determines:
  - Whether approved records [appear on Digital Collections](/metadata-documentation/dc/criteria/) based on **Approved use**:
    - **Can be used on NYPL website**: available globally
    - **Can be displayed on NYPL premises**: available from any computer connected to the internet at any Research or Branch location of the New York Public Library
    - **Can be displayed on NYPL premises :: [location]**: available from any computer connected to the internet at the location specified
  - Whether and how assets can be downloaded
- Rights metadata can be applied to MMS records in two ways:
  - Set at the record level, either through a local profile ([example](https://metadata.nypl.org/items/6549292?section=rights#:~:text=Rights%20specified%20at%20this%20level.)) or through a custom profile ([example](https://metadata.nypl.org/items/3044225?section=rights#:~:text=Rights%20specified%20in%20custom%20profile))
    - A local profile can only be set for one record, but a custom profile can be set for multiple records 
    - Any local profile can become a custom profile if saved as a reusable profile by Rights Clearance
  - Inherited from a higher container ([example](https://metadata.nypl.org/items/4642258?section=rights#:~:text=Rights%20information%20specified%20at%20a%20higher%20container%20level)) or collection ([example](https://metadata.nypl.org/items/3012441?section=rights#:~:text=Rights%20information%20specified%20at%20the%20collection%20level))
    - Local and custom profiles set at the record level are preferenced over inherited rights from a higher container or collection
- Rights information can be found on the **Overview** and **Rights and use** tabs of a record
  - The **Rights** section of the **Overview** tab indicates information about when rights were created or updated rights and by whom
  - The **Rights Profile** column of container and item lists on the **Overview** tab displays a symbol that indicates if and where rights are assigned
    - A checkmark (`✓`)  indicates that rights metadata is set at the record level ([example](https://metadata.nypl.org/collection/40346))
    - An `i` indicates that rights metadata is inherited from a higher container or collection ([example](https://metadata.nypl.org/collection/40232))
    - Dashes (`--`) indicate that rights have not been assigned at the record level and are not inherited from a higher container or collection ([example](https://metadata.nypl.org/collection/40346))
  - The **Rights and use** tab displays what is shown on the **Overview** tab as well as **Approved uses** and **Rights Research and Copyright Information Summary**
    - Codes used for the **Copyright status** in the **Rights Research and Copyright Information Summary** are defined in [metadata-database › Quick Reference › Rights Statements🔒](https://github.com/NYPL/metadata-database/blob/main/quick-reference.md#rights-statements)
  - MMS users with a **Rights Staff** and/or **Rights Admin** [user role](/metadata-documentation/system/accounts/#user-roles) will see more information on the **Rights and use** tab and throughout MMS than those who do not