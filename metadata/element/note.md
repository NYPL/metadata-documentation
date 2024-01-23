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
- Use [inclusive descriptive practices](/metadata-documentation/metadata/inclusive-reparative/)

{: .note }
> See [Reparative Description › Workflows (For MSU Staff)](/metadata-documentation/metadata/inclusive-reparative/#addressing-transcribed-title-elements) for workflows to follow in the event you wish to use the **Note** element to indicate description or content found to be harmful, biased, offensive, outdated, or inaccurate.

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
- Select **admin** for notes that should not appear publicly on [Digital Collections](/metadata-documentation/resources/glossary/#digital-collections)
  - Admin notes can be used for:
    - Identifying uncataloged material
      - Use `Uncataloged (YYYY-MM-DD INITIALS)`
    - Documenting [reparative description](/metadata-documentation/metadata/inclusive-reparative/#workflows-for-msu-staff) changes
    - Indicating known issues with digitized assets
    - Storing box and folder information from finding aid imports
      - Check with the division as to whether adding box and folder information to **Note (admin)** or **Location (Call number/Shelf Locator)** is preferred
      - It is not necessary to sign admin notes that contain box and folder information
  - Sign admin notes that you write yourself with `(YYYY-MM-DD INITIALS)`
    - Replace `YYYY-MM-DD` with the date in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format
    - Replace `INITIALS` with your initials (see [MMS Database › Quick Reference › User IDs 🔒](https://github.com/NYPL/metadata-tools/blob/master/_mms-database-and-sql-queries/mms-db_quick-reference.md#user-ids))
    - Wrap the signature in parenthesis with no other punctuation as consistent usage will allow staff to locate signed admin notes in the future
- If there is not an appropriate **Type** for the information in your respective note, use **content**
    - See [MARC 500](https://www.oclc.org/bibformats/en/5xx/500.html)
    - Do not use **Note** type **content** for individual contents of a resource, instead see [Table of Contents](/metadata-documentation/metadata/element/table-of-contents/) or [Abstract](/metadata-documentation/metadata/element/abstract/)

---

## See Also
- [Top-level Element: &lt;note&gt;](https://www.loc.gov/standards/mods/userguide/note.html) for official MODS documentation from the Library of Congress
- [MODS &lt;note&gt; Types](https://www.loc.gov/standards/mods/mods-notes.html) for a complete list of types