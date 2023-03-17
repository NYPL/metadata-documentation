---
layout: page
title: Title
permalink: /metadata/element/title/
parent: By Element
grand_parent: MMS › Metadata
nav_exclude: true
nav_order: 2
---

# Title
{: .d-inline .v-align-middle .no_toc .mr-2 }
Required
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
Repeatable
{: .d-inline .v-align-middle .label .label-green .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/titleinfo.html)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

A word, phrase, character, or group of characters, normally appearing in a resource, that names it or the work contained in it
{: .d-block .mt-2 .fs-6 .fw-300 }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Guidelines
- If a title appears on the resource, transcribe it into a title field
- If no title appears on the resource, devise a unique and descriptive title
    - Briefly describe the nature of resource, e.g. a map, or the subject of the resource, or both
    - Choice and format of title elements should be governed by the relevant [content standard](/metadata-documentation/metadata/guidelines/#content-standards)
    - Use [inclusive descriptive practices](/metadata-documentation/metadata/guidelines/#inclusive-and-reparative-description)
    - See [By Material](/metadata-documentation/metadata/material/) and [By Division](/metadata-documentation/metadata/division/) for guidelines on constructing titles specific to corresponding resources

## Workflows

### Addressing Incorrect or Offensive Titles

The following workflow details how to provide new titles for resources that have titles that are incorrect, offensive, not descriptive, or have other issues, while maintaining a record of the source of the original title and why it has been deprecated

1. Add a new **Title** element that addresses the issues in the original **Title** element (see [Guidelines](#guidelines))
    1. If correcting only a specific portion of the text, enclose the corrected text in brackets, e.g. "[their]" to replace "[thier]"
    1. Check **Primary** and **Supplied** for the new **Title** element
1. In the original **Title** element:
    1. Uncheck **Primary**
    1. In the **Part Name** box, enter the source of the original title in square brackets (i.e. "[caption title]")
1. If further clarification is needed about the original or updated title, add a [Note](/metadata-documentation/metadata/element/note/) with type **Content**

{: .note-title }
> Example
>
> The official caption of a photograph incorrectly identified the people in the photograph:
> [https://metadata.nypl.org/items/4951434?section=desc_md 🔒](https://metadata.nypl.org/items/4951434?section=desc_md)


{: .note-title }
> Example
>
> The division wished to add a more descriptive title than what appeared on the image:
> [https://metadata.nypl.org/items/6232674?section=desc_md 🔒](https://metadata.nypl.org/items/6232674?section=desc_md)


## Subelements

---

### Title
{: .d-inline .v-align-middle .mr-2 }
Required
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/titleinfo.html#title)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_A word, phrase, character, or group of characters that constitutes the chief title of a resource, i.e., the title normally used when citing the resource_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Remove punctuation at the end of the **Title**—such as periods or colons—unless part of the title as seen on the item
- Remove brackets enclosing the entirety of the **Title**
    - If brackets indicated the title was devised and not transcribed from the resource, see [**Supplied**](#supplied)
- Remove any [general material designation](/metadata-documentation/resources/glossary/#general-material-designation) from the **Title**
- See [MARC 245](https://www.oclc.org/bibformats/en/2xx/245.html)

---

### Subtitle
{: .d-inline .v-align-middle .mr-2 }
Recommended if applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/titleinfo.html#subtitle)
{: .d-inline .v-align-middle .text-zeta .ml-2 }
_A word, phrase, character, or group of characters that contains the remainder of the title information after the title proper_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Move any text that follows a colon in the **Title** to the **Subtitle**
- Split the **Title** if it is exceptionally long by moving anything not deemed the primary title to **Subtitle**
- Remove any punctuation that separates the **Title** and **Subtitle**
- See [MARC 245$b](https://www.oclc.org/bibformats/en/2xx/245.html#subfieldb)

---

### Part Number
{: .d-inline .v-align-middle .mr-2 }
Required if Applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/titleinfo.html#partnumber)
{: .d-inline .v-align-middle .text-zeta .ml-2 }
_A part or section number of a title_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Add a **Part Number** to indicate sequencing in any form (e.g., "Book two," "Part 1," or "Supplement A")
- Record all numbering/sequencing in a single **Part Name** using a comma to separate multiple numbering (e.g., "Volume 1, Issue 2")
- Remove any punctuation that separates **Part Number** from other subelements
- See [MARC 245$n](https://www.oclc.org/bibformats/en/2xx/245.html#subfieldn)

---

### Part Name
{: .d-inline .v-align-middle .mr-2 }
Required if Applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/titleinfo.html#partname)
{: .d-inline .v-align-middle .text-zeta .ml-2 }
_A part or section name of a title_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Add a **Part Name** to record a name designation for a part or section of a work
- Remove any punctuation that separates **Part Name** from other subelements
- See [MARC 245$p](https://www.oclc.org/bibformats/en/2xx/245.html#subfieldp)

---

## Attributes

---

### Primary
{: .d-inline .v-align-middle .mr-2 }
Required if Applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/attributes.html#usage)
{: .d-inline .v-align-middle .text-zeta .ml-2 }
_Used for a repeated element to declare that a particular instance of the element is most important_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Check **Primary** for <u>one</u> **Title** element if more than one **Title** element exists for a record
- If **Primary** is checked for a **Title** element, do not use the **Type** dropdown on that title

---

### Supplied
{: .d-inline .v-align-middle .mr-2 }
Recommended if Applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/attributes.html#supplied)
{: .d-inline .v-align-middle .text-zeta .ml-2 }
_Indicates whether the content of the element has been supplied from external sources, or from a source other than the ones prescribed by the content standard used_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- If no title appears on the resource, devise a unique and descriptive title according the [guidelines](#guidelines) and check **Supplied**
- Do not check **Supplied** for the following as they are not replacements for missing titles
    - Collection titles
    - Container titles
    - Titles describing correspondence, manuscripts, or other archival materials
- Do not enclose titles checked as **Supplied** in brackets

---

### Type
{: .d-inline .v-align-middle .mr-2 }
Strongly Recommended if Applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/titleinfo.html#type)
{: .d-inline .v-align-middle .text-zeta .ml-2 }
_Identifies what type of title is recorded_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- When there are multiple titles, **Type** is strongly recommended for all **Title** elements except for the **Title** marked **Primary**
- Various title forms may be entered to enhance the possibility for discovery of a resource for:
    - Single titles within a multi-titled resource
    - To bring out titles contained within a main title
    - To spell out abbreviated terms or numerals
    - To modernize archaic forms
    - To reformat erroneous title information
    - To provide a descriptive title when the main title is not descriptive
- Select the **Type** according to the following definitions:
    - **Abbreviated**: title as abbreviated for indexing or identification
        - Select the appropriate choice from the **Authority** dropdown
        - See [MARC 210](https://www.oclc.org/bibformats/en/2xx/210.html)
        - See [Abbreviated Title Source Codes](https://www.loc.gov/standards/sourcelist/abbreviated-title.html)
    - **Translated**: translation or transcription of the main title
        - Record translations of titles in two separate title elements rather than expressing their equivalency within a single field (e.g. “Chinese lives = Huaxia ren sheng”)
        - Select the appropriate **Language** from the dropdown for the corresponding **Title** element
        - See [MARC 242](https://www.oclc.org/bibformats/en/2xx/242.html) and [MARC 246](https://www.oclc.org/bibformats/en/2xx/246.html)
    - **Alternative**: varying form of the title if it contributes to the further identification of the item
        -  See [MARC 246](https://www.oclc.org/bibformats/en/2xx/246.html) and [MARC 740](https://www.oclc.org/bibformats/en/7xx/740.html)
    - **Uniform**: used as a main entry in a bibliographic record when a work has appeared under varying titles, necessitating that a particular title be chosen to represent the work
        -  Select the appropriate choice (LCNAF or LCSH) from the **Authority** dropdown
        -  See [MARC 130](https://www.oclc.org/bibformats/en/1xx/130.html), [MARC 240](https://www.oclc.org/bibformats/en/2xx/240.html), and [MARC 730](https://www.oclc.org/bibformats/en/7xx/730.html)

---

### Language
{: .d-inline .v-align-middle .mr-2 }
Recommended
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/attributes.html#lang)
{: .d-inline .v-align-middle .text-zeta .ml-2 }
_Indicates the language of the content of an element_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Select the language of the title from the dropdown
- Do not use the **Language** subelement of **Title** to record the language of the content of the resource
    - Use the [**Language**](/metadata-documentation/metadata/element/language/#language) subelement within the [**Language**](/metadata-documentation/metadata/element/language/) element to record the language of the content of the resource
- If you are unsure of the language of the title, leave **Language** blank or select **Undetermined**

---

### Script
{: .d-inline .v-align-middle .mr-2 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/attributes.html#script)
{: .d-inline .v-align-middle .text-zeta .ml-2 }
_Indicates the script used for an element_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Select the script of the title from the dropdown if it is a non-Roman script or not the default script of the title’s language
- Do not use the **Script** subelement of **Title** to record the script of the content of the resource
    - Use the [**Script**](/metadata-documentation/metadata/element/language/#script) subelement within the [**Language**](/metadata-documentation/metadata/element/language/) element to record the script of the content of the resource
- If you are unsure of the script of the title, leave **Script** blank or select **Undetermined**

---


## See Also
- [Top-level Element: &lt;titleInfo&gt;](https://www.loc.gov/standards/mods/userguide/titleinfo.html) for official MODS documentation from the Library of Congress
- [By Material](/metadata-documentation/metadata/material/) for access to **Title** element guidance for Clippings, Periodicals, etc.