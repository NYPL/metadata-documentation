---
layout: page
title: Physical Description
permalink: /metadata/element/physical-description/
parent: By Element
grand_parent: MMS › Metadata
nav_exclude: true
nav_order: 10
---

# Physical Description
{: .d-inline .v-align-middle .no_toc .mr-2 }
Repeatable
{: .d-inline .v-align-middle .label .label-green .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/physicaldescription.html)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

Physical characteristics of the resource
{: .d-block .mt-2 .fs-6 .fw-300 }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Purpose
- To provide information about the physical details of the analog source object including physical format or medium, length, number, size, or duration
- To provide a means of disambiguation when multiple versions of a resource are held by the library

## Guidelines
- See [subelements](#subelements)

## Subelements

---

### Form
{: .d-inline .v-align-middle .mr-2 }
Repeatable
{: .d-inline .v-align-middle .label .label-green .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/physicaldescription.html#form)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_A particular physical presentation of a resource, including the physical form or medium of material for a resource_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Use **Form** to describe the physical carrier of the content
- Guidance for which **Form** terms to use can be found on the work-in-progress [Genre + Form + Extent 🔒](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=187807178) spreadsheet
- When adding a new **Form** element, start by searching within the available [controlled vocabularies](/metadata-documentation/metadata/guidelines/#controlled-vocabularies) using the MMS authorities module
    - Select the radio button for **Authority data search**
    - Click **Select from controlled terms** to bring up the authorities module
    - Look up the form you wish to add in the search box
    - For all materials excluding audio and moving image (non-AMI), select a **Form** that is more granular than [**Genre**](/metadata-documentation/metadata/element/genre/)
    - The order of preference for adding additional **Form** values absent from the [Genre + Form + Extent 🔒](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=187807178) spreadsheet is:
        - LC Thesaurus for Graphic Materials (LCTGM)
        - LC Genre/Form Thesaurus (LCGFT)
        - Art and Architecture Thesaurus (AAT)
    - For audio and moving image (AMI), only terms from the **Form (AMI) tab** of the [Genre + Form + Extent 🔒](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=187807178) spreadsheet may be used
    - To verify a result is appropriate, click the linked **Authorized Term** to view the corresponding record in the source authority
    - Once you have chosen the controlled term, click the **Use this term** button
    - Do not add **Free text** values for **Form**
- When the analog source is a reproduction of the original (e.g., microform), **Form** is required

---

### Extent
{: .d-inline .v-align-middle .mr-2 }
Repeatable
{: .d-inline .v-align-middle .label .label-green .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/physicaldescription.html#extent)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_A statement about the physical extent of the resource, in terms of units of measurement and material_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Format the **Extent** string according to the relevant [content standard](/metadata-documentation/metadata/guidelines/#content-standards)
    - Include the extent, other physical details, and dimensions
- See [MARC 300](https://www.oclc.org/bibformats/en/3xx/300.html)

---

### Note
{: .d-inline .v-align-middle .mr-2 }
Repeatable
{: .d-inline .v-align-middle .label .label-green .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/physicaldescription.html#note)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_General textual information about the physical description of a resource_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Select a note **Type** for all notes
    - See [MODS &lt;physicalDescription&gt;&lt;note&gt;](https://www.loc.gov/standards/mods/mods-notes.html#:~:text=MODS%20%3CphysicalDescription%3E%3Cnote%3E) for a complete list of types
        - Refer to **MARC Equivalent** column to see corresponding MARC field for each type
        - Look up fields in the [OCLC Bibliographic Formats and Standards](https://www.oclc.org/bibformats/en.html) for more details documentation
- Format the **Note** string according to the relevant [content standard](/metadata-documentation/metadata/guidelines/#content-standards)
    - Include textual information about the physical details of the source object
- A separate **Note** subelement should be used for each distinct note
- Always select an appropriate **Type** from the dropdown menu
- For notes describing the content, provenance, or other details, use the [Note](/metadata-documentation/metadata/element/note/) element at the record level

---

## See Also
- [Top-level Element: &lt;physicalDescription&gt;](https://www.loc.gov/standards/mods/userguide/physicaldescription.html) for official MODS documentation from the Library of Congress