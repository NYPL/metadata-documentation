---
layout: page
title: Manuscripts and Archives Division
permalink: /division/manuscripts-archives/
parent: By Division
grand_parent: MMS › Metadata
nav_exclude: true
---

<style>code { white-space : pre-wrap !important; word-break: break-word; }</style>

# Manuscripts and Archives Division
{: .no_toc }

Provides guidelines for metadata describing material from the Manuscripts and Archives Division in the Metadata Management System (MMS)

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Guidelines

{: .note }
Materials described by the [Miscellaneous personal name files D-Z](https://archives.nypl.org/mss/2016) finding aid are technically uncataloged but do not require special permission from the Manager, Metadata Services for [metadata to be created](/metadata-documentation/workflows/creating/) in MMS.

---

### Record Structure
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Record Types →](/metadata-documentation/metadata/record-type/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For materials itemized in the [Miscellaneous personal name files D-Z](https://archives.nypl.org/mss/2016) finding aid:
  - Do not import the finding aid into MMS
  - Create a new collection record in MMS based on the corresponding reference item record in the [collection](https://qa-metadata.nypl.org/collection/129052) that has been imported into [MMS QA](/metadata-documentation/resources/glossary/#mms-qa)
  - Ensure metadata elements align with the additional relevant guidelines outlined on this page

---

### Title
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/title/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For collection records that correspond to materials itemized in the [Miscellaneous personal name files D-Z](https://archives.nypl.org/mss/2016) finding aid:
  - **Title**: `Miscellaneous personal name files`
  - **Subtitle**: enter the creator name in direct order
  - E.g. [Miscellaneous personal name files: Sir Arthur Conan Doyle](https://metadata.nypl.org/collection/70950?section=desc_md#:~:text=Title-,Miscellaneous%20personal%20name%20files%3A%20Sir%20Arthur%20Conan%20Doyle,-Name)

---

### Identifier
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/identifier/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For collection records that correspond to materials itemized in the [Miscellaneous personal name files D-Z](https://archives.nypl.org/mss/2016) finding aid:
  - Enter [Archives EAD ID](/metadata-documentation/metadata/element/identifier/archives-ead/) based on the corresponding reference item record in the [MMS QA](/metadata-documentation/resources/glossary/#mms-qa) [collection](https://qa-metadata.nypl.org/collection/129052) and set it to inherit
  - Enter [Archives Components ID](/metadata-documentation/metadata/element/identifier/archives-components/) in the collection record ****based on the corresponding reference item record in the [MMS QA](/metadata-documentation/resources/glossary/#mms-qa) [collection](https://qa-metadata.nypl.org/collection/129052)

---

### Note
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/note/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For collection records that correspond to materials itemized in the [Miscellaneous personal name files D-Z](https://archives.nypl.org/mss/2016) finding aid:
  - Add a **Note** element with the **Type**: **admin** by copying and pasting the following text:
    ```
    Collection is component of "Miscellaneous personal name files D-Z" (https://archives.nypl.org/mss/2016#archives_component_id) (YYYY-MM-DD INITIALS)
    ```
    - Replace `YYYY-MM-DD` with the date in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format
    - Replace `INITIALS` with your initials (see [MMS Database › Quick Reference › User IDs 🔒](https://github.com/NYPL/metadata-tools/blob/master/_mms-database-and-sql-queries/mms-db_quick-reference.md#user-ids))
    - Set the element to inherit
    - E.g. [`Collection is component of "Miscellaneous personal name files D-Z"(http://archives.nypl.org/mss/2016#c791494) (2024-03-18 SAA)`](http://archives.nypl.org/mss/2016#c791494)
  - Add a **Note** element with the **Type**: **admin** by copying and pasting the following text:
    ```
    [LAST NAME] MMS QA container for reference: [QA CONTAINER URL] (YYYY-MM-DD INITIALS)
    ```
    - Replace `YYYY-MM-DD` with the date in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format
    - Replace `INITIALS` with your initials (see [MMS Database › Quick Reference › User IDs 🔒](https://github.com/NYPL/metadata-tools/blob/master/_mms-database-and-sql-queries/mms-db_quick-reference.md#user-ids))
    - Set the element to inherit
    - E.g. [`Doyle MMS QA item for reference: https://qa-metadata.nypl.org/items/6379914 (2024-03-18 SAA)`](https://qa-metadata.nypl.org/items/6379914)

---

### Location
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/location/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For collection records that correspond to materials itemized in the [Miscellaneous personal name files D-Z](https://archives.nypl.org/mss/2016) finding aid:
  - If a call number beginning with `MssCol` is available, add it as the **Call number / Shelf Locator**
    - E.g. [`MssCol 9542`](https://metadata.nypl.org/collection/70950?section=desc_md#:~:text=MSS%2C%20Shelf%20locator%3A-,MssCol%209542,-Highlighted%20elements%20are)


---

## See Also

- [Manuscripts and Archives Division (Internal Documentation) 🔒](https://docs.google.com/document/d/1hTXl5PMCSzmpdIMtOkxRwDagPeIxqSOZQLwRCGVI1ao/edit) for the respective [MSU Liason's 🔒](https://docs.google.com/spreadsheets/d/1P-YDJigon640fTCLP4Ig4-zmzqrX88v5M24ShuxFNVY/edit?gid=0) internal documentation and notes related to the Manuscripts and Archives Division