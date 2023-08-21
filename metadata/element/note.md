---
layout: page
title: Note
permalink: /metadata/element/note/
parent: By Element
grand_parent: MMS › Metadata
nav_exclude: true
nav_order: 14
---

<style>code { white-space : pre-wrap !important; word-break: break-word; }</style>

# Note
{: .d-inline .v-align-middle .no_toc .mr-2 }
Repeatable
{: .d-inline .v-align-middle .label .label-green .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/note.html)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

General textual information relating to a resource
{: .d-block .mt-2 .fs-6 .fw-300 }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Purpose
- To provide additional information about the resource that cannot be adequately captured in other fields

## Guidelines
- Use the free text field to enter a note
- Ensure a note [**Type**](#type) is selected
- For notes describing the physical details of the original object, use the [Note](/metadata-documentation/metadata/element/physical-description/#note) subelement of [Physical Description](/metadata-documentation/metadata/element/physical-description/)
- Use [inclusive descriptive practices](/metadata-documentation/metadata/guidelines/#inclusive-and-reparative-description)

## Workflows

### Flagging Harmful or Difficult Content

{: .note }
The following workflow details how to add a **Note** for instances where the _content_ of the resource may be considered harmful, offensive, or have other issues. For additional workflows and general practices related to instances where _description_ may be considered harmful or offensive, see [Inclusive and Reparative Description](/metadata-documentation/metadata/guidelines/#inclusive-and-reparative-description).

1. Consult with relevant [Division staff 🔒](https://docs.google.com/spreadsheets/d/1P-YDJigon640fTCLP4Ig4-zmzqrX88v5M24ShuxFNVY/edit#gid=0&range=F2:F37) if you encounter harmful or offensive content on Digital Collections or it is [reported](/metadata-documentation/workflows/remediations/feedback/) to you
    1. Division staff may request one or both of the following steps:
        1. The resource can be suppressed from public view in Digital Collections (resources cannot be removed from MMS)
        1. A note can be added to the descriptive metadata
    1. If the Division requests suppression:
        1. Navigate to the **Rights and use** tab of an item record
        1. Select **Suppress** from website
        1. Do not select a **Reason**
        1. Add an explanation in the **Notes** field of the suppression prompt, e.g. `division requested suppression for harmful content [add date]`
        1. Click the **Suppress record** button
    1. If the Division requests a note:
        1. Add a new **Note** element by copying and pasting the following text:
        ```
This record may contain content that is harmful or difficult to view. For more information, please refer to NYPL's Statement on Potentially Harmful Content for Digital Collections: https://digitalcollections.nypl.org/about#nypl_harmful_content_statement
        ```
            1. Add the above text without alteration as consistent usage will allow staff to locate harmful content records in the future
            1. If the above text does not seem applicable, discuss with the [Manager, Metadata Services](/metadata-documentation/contact/#our-team)
        1. Select **content** as the **Type**

---

## Attributes

---

### Type
{: .d-inline .v-align-middle .mr-2 }
Required if Applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/note.html#type)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_Identifies what type of note is recorded_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Select a **Type** for every **Note** element
    - See [MODS &lt;note&gt; Types](https://www.loc.gov/standards/mods/mods-notes.html) for a complete list of types
    - Refer to **MARC Equivalent** column to see corresponding MARC field for each type
    - Look up fields in the [OCLC Bibliographic Formats and Standards](https://www.oclc.org/bibformats/en.html) for more detailed documentation
- **Admin** notes do not appear publicly on [Digital Collections](/metadata-documentation/resources/glossary/#digital-collections) and should be used to record information such as:
    - Identifying uncataloged material
    - Documenting reparative description changes
    - Known issues with digitized assets
- Box and folder information from finding aid imports may appear in [Call number/Shelf Locator](/metadata-documentation/metadata/element/location/#call-number--shelf-locator) in the [Location](/metadata-documentation/metadata/element/location/) element or a **Note** with **admin** as the **Type**
    - Check with the division as to whether adding box and folder information to **Note** (**admin**) or **Location** (**Call number/Shelf Locator**) is preferred
- If there is not an appropriate **Type** for the information in your respective note, use **content**
    - See [MARC 500](https://www.oclc.org/bibformats/en/5xx/500.html)
    - Do not use **Note** type **content** for individual contents of a resource, instead see [Table of Contents](/metadata-documentation/metadata/element/table-of-contents/) or [Abstract](/metadata-documentation/metadata/element/abstract/)

---

## See Also
- [Top-level Element: &lt;note&gt;](https://www.loc.gov/standards/mods/userguide/note.html) for official MODS documentation from the Library of Congress
- [MODS &lt;note&gt; Types](https://www.loc.gov/standards/mods/mods-notes.html) for a complete list of types