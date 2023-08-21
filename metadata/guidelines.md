---
layout: page
title: General Guidelines
permalink: /metadata/guidelines/
parent: MMS › Metadata
nav_order: 2
---

{: .highlight-title }
> 🚧 Under Construction
>
> This page is still being developed. Links to legacy documentation may appear to facilitate our migration process. [Contact us](/metadata-documentation/contact/) with any questions or feedback.

# General Guidelines
{: .no_toc }

This page provides broader guidance on standards and best practices for metadata in the context of the Metadata Management System (MMS)

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

## Inheritance
- The inheritance functionality within MMS facilitates efficient metadata creation by eliminating repetitive re-keying of data
- Inheritance should be carefully considered when used
- All [elements](/metadata-documentation/metadata/element/) in the **Descriptive metadata** tab of a collection or container records have a corresponding **Inheritable** checkbox
- Inherited metadata elements can be found in the **Descriptive metadata** tab of a container or item record under **Inherited elements**
    - Elements in gray are inherited from another record
    - Yellow highlighted elements are inheritable from a given record
    - Click the the **Override** link in the **Inherited elements** section to disinherit a metadata element
        - If **Override** is clicked on a collection or container, the metadata element will also be disinherited from all records contained by that record

## Minimum Metadata Requirements
MMS item records must include the following seven descriptive metadata elements/subelements, either assigned or inherited, to be approved to appear on Digital Collections (see [Approvals](/metadata-documentation/workflows/approvals/))
1. [Title](/metadata-documentation/metadata/element/title/)
1. [Type of Resource](/metadata-documentation/metadata/element/type-of-resource/)
1. [Identifier](/metadata-documentation/metadata/element/identifier/)
1. [Date](/metadata-documentation/metadata/element/origin-info/#date) (sublement of [Origin Info](/metadata-documentation/metadata/element/origin-info/))
1. [Genre](/metadata-documentation/metadata/element/genre/)
1. [Location](/metadata-documentation/metadata/element/physical-location/)
1. [Language](/metadata-documentation/metadata/element/language/) (if applicable)

Rights
------

- Rights metadata determines:
    - Whether approved records [appear on Digital Collections](/metadata-documentation/dc/criteria/) based on **Approved use**:
        - **Can be used on NYPL website**: available globally
        - **Can be displayed on NYPL premises**: available from any computer connected to the internet at any Research or Branch location of the New York Public Library
        - **Can be displayed on NYPL premises :: location, LPA-wide**: available from any computer connected to the internet at the Library for the Performing Arts
    - Whether and how assets can be downloaded
- Rights information can be found on the **Overview** and **Rights and use** tabs of a record
    - The **Rights** section of the **Overview** tab indicates whether rights are set at that record's level or inherited as well as information about when rights were created or updated rights and by whom
    - The **Rights and use** tab displays what is shown on the **Overview** tab as well as **Approved uses** and a **Rights Research and Copyright Information Summary**
        - Codes used for the **Copyright status** in the **Rights Research and Copyright Information Summary** are defined on the [Rights Codes Cheat Sheet](https://confluence.nypl.org/display/DIG/Rights+Codes+Cheat+Sheet)
- Rights are added and maintained by [Copyright and Information Policy](/metadata-documentation/resources/glossary/#copyright-and-information-policy)

## Inclusive and Reparative Description

{: .note }
In addition to the general workflows and best practices described below, the Metadata Services Unit leads and participates in several initiatives related to inclusive and reparative description, see [Projects](/metadata-documentation/projects/) for more details.

### Workflows
- [Addressing Incorrect or Offensive Titles](/metadata-documentation/metadata/element/title/#addressing-incorrect-or-offensive-titles)
- [Flagging Harmful or Difficult Content](/metadata-documentation/metadata/element/note/#flagging-harmful-or-difficult-content)

### Describing People
- If describing the race or ethnicity of any one individual person in [**Title**](/metadata-documentation/metadata/element/title/) or [**Note**](/metadata-documentation/metadata/element/note/), include the race or ethnicity for all people depicted in the resource
    - Do not assume race or ethnicity of people; research how they self-identified where possible
    - Use linguistically similar qualifiers in description, e.g. "black women" and "white women" or "African American women" and "Caucasian women"
    - Omit gendered language
    - Do not describe only women as pretty or comment on their appearance, hair, or clothing while not describing men in a similar fashion