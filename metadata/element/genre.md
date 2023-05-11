---
layout: page
title: Genre
permalink: /metadata/element/genre/
parent: By Element
grand_parent: MMS › Metadata
nav_exclude: true
nav_order: 8
---

# Genre
{: .d-inline .v-align-middle .no_toc .mr-2 }
Required
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
Repeatable
{: .d-inline .v-align-middle .label .label-green .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/genre.html)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

A term or terms that designate a category characterizing a particular style, form, or content, such as artistic, musical, literary composition, etc.
{: .d-block .mt-2 .fs-6 .fw-300 }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Purpose
- To describe the nature of the content or function of the resource
- To provide a greater level of specificity than [**Type of Resource**](/metadata-documentation/metadata/element/type-of-resource/) using a defined set of values drawn from controlled vocabularies

## Guidelines
- Guidance for which **Genre** terms to use can be found on the work-in-progress [Genre + Form + Extent 🔒](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=187807178) spreadsheet
  - For all materials excluding audio and moving image (AMI), use a **Genre** that describes what the digitized resource is (e.g. Photographs, Songbooks, Paintings, Correspondence, etc.)
  - For AMI materials, use a **Genre** that describes what the sound recording or moving image is capturing (e.g., Interviews, Lectures, Oral histories, etc.) or what kind of sound recording or moving image the resource is (e.g., Demo recordings, Documentary films, Radio commercials, etc.)
- When adding a new **Genre** element, start by searching the MMS authorities module
  - Select the radio button for **Authority data search**
  - Click **Select from controlled terms** to bring up the authorities module
  - Look up the genre you wish to add in the search box
  - The order of preference for for adding additional **Genre** values not on the [Genre + Form + Extent 🔒](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=187807178) spreadsheet is:
    - For materials excluding AMI:
    - LC Thesaurus for Graphic Materials (LCTGM)
    - LC Genre/Form Thesaurus (LCGFT)
    - Library of Congress Subject Heading (LCSH)
  - To verify a result is appropriate, click the linked **Authorized Term** to view the corresponding record in the source authority
  - Once you have chosen the controlled term, click the **Use this term** button
- Do not add **Free text** values for **Genre**

---

## Attributes

---

###  Primary
{: .d-inline .v-align-middle .mr-2 }
Required if Applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/attributes.html#usage)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_Used for a repeated element to declare that a particular instance of the element is most important_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Check **Primary** for <u>one</u> **Genre** element if more than one **Genre** element exists for a record

---

## See Also
- [Top-level Element: &lt;Genre&gt;](https://www.loc.gov/standards/mods/userguide/genre.html) for official MODS documentation from the Library of Congress
- [Type of Resource](/metadata-documentation/metadata/element/type-of-resource/) for guidelines on adding an element that describes a resource in a more general sense
- [Physical Description / Form](/metadata-documentation/metadata/element/physical-description/#form) for guidelines on adding an subelement that describes the more specific physical format of a resource
[Genre + Form + Extent 🔒](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit) for a draft/work-in-progress reference to inform your selection of a genre term