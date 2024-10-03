---
layout: page
title: Archival Collections
permalink: /metadata/material/archival-collections/
parent: By Material
grand_parent: MMS › Metadata
nav_exclude: true
---

# Archival Collections
{: .no_toc }

Provides guidelines for metadata specific to archival collections described in the Metadata Management System (MMS)

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Guidelines

---

### Record Structure
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Record Types →](/metadata-documentation/metadata/record-type/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- Record structure for archival collections should mirror the hierarchy established by the [finding aid](/metadata-documentation/workflows/importing/finding-aids/)
  - Importing EAD-encoded finding aids will replicate the structure of the finding aid within MMS
    - [Convert items](/metadata-documentation/workflows/remediation/restructuring/#converting-items) at the lowest level of the hierarchy in the finding aid that have imported as items into containers as needed
  - Importing finding aids that are only available as a PDF will create an item record
    - In cases where the full finding aid structure is not imported as it is not EAD-encoded, create containers and items within the collection as appropriate to replicate the structure outlined in the PDF
    - In cases where the finding aid represents a fully digitized single-item collection (e.g., the [Augustus Porter daybook 🔒](https://metadata.nypl.org/items/6120514)), the record should remain a standalone item
  - See [Importing Finding Aids](/metadata-documentation/workflows/importing/finding-aids/) for additional guidelines and steps

---

### Title
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/title/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- Do not modify titles imported or replicated from the finding aid unless requested by the division

---

### Identifier
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/identifier/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For all collection records:
    - Set the [**MSS Unit ID**](/metadata-documentation/metadata/element/identifier/mss-unit/) to be **Inheritable**
    - Set the [**NYPL catalog ID (B-number)**](/metadata-documentation/metadata/element/identifier/bnumber/) to be **Inheritable**
- For all records that correspond to an EAD-encoded finding aid:
  - For collection records that correspond to an EAD-encoded finding aid:
    - Ensure the presence of an [**Archives Collections ID**](/metadata-documentation/metadata/element/identifier/archives-collections/)
    - Do not set the [**Archives Collections ID**](/metadata-documentation/metadata/element/identifier/archives-collections/) to be **Inheritable**
  - For container and item records that correspond to an EAD-encoded finding aid:
    - Ensure the presence of an [**Archives EAD ID**](/metadata-documentation/metadata/element/identifier/archives-ead/), either:
      - Assigned to the appropriate container record and set to to be **Inheritable** so that it appears on all child records
      - Assigned to the appropriate item record

---

### Type of Resource
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/type-of-resource/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For collection records:
  - Add any appropriate **Type of Resource**
  - Check **primary** for the predominant **Type of Resource** of the collection

---

### Genre
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/genre/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For container records that have a genre term as a [**Title**](/metadata-documentation/metadata/element/title/) (e.g. `Correspondence` or `Manuscripts`):
  - Add the appropriate **Genre** element from the [Genre + Form + Extent 🔒](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=187807178) spreadsheet and set to be **Inheritable**

---

### Language
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/language/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For collection records:
  - Add every **Language** represented in the collection based on the **Language** field of the finding aid
  - Check **primary** for the predominant **Language** of the collection
  - If the entire collection is a single language, set the **Language** to be **Inheritable**

---

### Physical Description
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/physical-description/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- If no **Physical Description** element was imported, review [**Note**](#note) elements to determine if any should be relocated to a **Physical Description** element
- Review imported **Physical Description** elements to determine if any should be relocated to another element such as a [**Note**](#note)

---

#### Form
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Subelement →](/metadata-documentation/metadata/element/physical-description/#form)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- A **Form** element is required for analog sources that are reproductions of the original such as microform
  - If an entire archival collection is the same form, add a **Form** element to the collection record and set it to be **Inheritable**

---

### Subject
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/subject/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For collection records:
  - If a subject is appropriate for the entire collection, set the **Subject** to be **Inheritable**
  - Review complex subject headings that have been imported to ensure the correct **Subject** [subelement](/metadata-documentation/metadata/element/subject/#subelements) is in use for each component
    - E.g. when importing a finding aid with the complex subject heading `United States -- History -- Spanish-American War, 1898`, each component is imported into a [subelement](/metadata-documentation/metadata/element/subject/#subelements) based on the type of the first component, in this case [**Geographic**](/metadata-documentation/metadata/element/subject/#geographic)
    - In this example, `History` and `Spanish-American War, 1898` are imported as [**Geographic**](/metadata-documentation/metadata/element/subject/#geographic) subelements and should be manually re-added as [**Topic**](/metadata-documentation/metadata/element/subject/#topic) subelements

---

### Note
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/note/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- Review imported **Note** elements to determine if any should be relocated to another element, e.g.:
  - A note containing `31 boxes` should be relocated to the [**Extent**](/metadata-documentation/metadata/element/physical-description/#extent) subelement of the [**Physical Description**](/metadata-documentation/metadata/element/physical-description/) element
  - A summary of the series or component content should be relocated to the [**Abstract**](/metadata-documentation/metadata/element/abstract/) element
- For container records:
  - Set any **admin** note containing box and folder information to be **Inheritable**

---

## See Also

- [Importing Finding Aids](/metadata-documentation/workflows/importing/finding-aids/) for the workflow of creating records in MMS by importing metadata from finding aids found in the Archives Portal