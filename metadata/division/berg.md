---
layout: page
title: Berg Collection
permalink: /division/berg/
parent: By Division
grand_parent: MMS › Metadata
nav_exclude: true
---

<style>code { white-space : pre-wrap !important; word-break: break-word; }</style>

# Berg Collection
{: .no_toc }

Provides guidelines for metadata describing material from the Berg Collection in the Metadata Management System (MMS)

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Guidelines

{: .note }
Materials described in the [Dictionary catalog of the Henry W. and Albert A. Berg Collection of English and American literature](https://catalog.hathitrust.org/Record/102778714) or itemized in the [Berg Collection Uncataloged Manuscripts](https://archives.nypl.org/brg/19347) finding aid are technically uncataloged but do not require special permission from the Manager, Metadata Services for [metadata to be created](/metadata-documentation/workflows/creating/) in MMS.

---

### Record Structure
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Record Types →](/metadata-documentation/metadata/record-type/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For printed books:
  - Unless otherwise requested by the division, records for printed books held by the Berg Collection should be located in the [Berg Collection printed books](https://metadata.nypl.org/collection/79490) collection
  - Structure the item or container record for an individual edition or copy of a book within a container for that author
    - For fully-digitized books:
```
    | -- Collection = Berg Collection printed books
      | -- Container = container for works by author
        | -- Item = book
```
    - For partially-digitized books:
```
  | -- Collection = Berg Collection printed books
    | -- Container = container for works by author
      | -- Container = book
        | -- Item = page(s)
```
    - Re-order the author containers within the collection as needed to maintain alphabetical order
  - Alternately, if requested by the division, printed books may located in the [Miscellaneous](https://metadata.nypl.org/containers/510234?section=overview) container as printed books in a container indicating whether the book is about or owned by a particular author
- For uncataloged manuscripts itemized in the [Berg Collection Uncataloged Manuscripts](https://archives.nypl.org/brg/19347) finding aid:
  - Do not import the finding aid into MMS
  - Create a new collection record in MMS based on the corresponding reference item record in the [collection](https://qa-metadata.nypl.org/collection/129034) that has been imported into [MMS QA](/metadata-documentation/resources/glossary/#mms-qa)
  - Ensure metadata elements align with the additional relevant guidelines outlined on this page

---

### Title
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/title/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For printed books:
  - For container records representing an author:
    - Enter the name of the author in indirect order
    - E.g. [`Baldwin, James`](https://metadata.nypl.org/containers/510233?section=desc_md#:~:text=Title-,Baldwin%2C%20James,-Type%20of%20Resource)
  - To disambiguate two editions of the same book represented by a container or item record:
    - **Title**: enter the book title
    - **Part Number**: enter the publication year and enclose in brackets
    - E.g. [`Giovanni's room [1977]`](https://metadata.nypl.org/containers/500614?section=desc_md#:~:text=Giovanni%27s%20room%20%5B1977%5D)
  - To disambiguate two copies of the same edition of a book represented by a container or item record:
    - **Title**: enter the book title
    - **Part Number**: enter `copy` followed by the copy number and enclose in brackets
    - E.g. [`Evelina, or, A young lady's entrance into the world [copy 1]`](https://metadata.nypl.org/containers/511575?section=desc_md#:~:text=Evelina%2C%20or%2C%20A%20young%20lady%27s%20entrance%20into%20the%20world%20%5Bcopy%201%5D)
  - To disambiguate multiple editions and copies of a book represented by a container or item record:
    - **Title**: enter the book title
    - **Part Number**: enter the publication year, a comma separator, and `copy` followed by the copy number and enclose in brackets
    - E.g. [`Ulysses, [1922, copy 2]`](https://metadata.nypl.org/containers/510096?section=desc_md#:~:text=Ulysses%20%5B1922%2C%20copy%202%5D)
  - See [By Material › Books › Title](/metadata-documentation/metadata/material/books/#title) for additional guidelines
- For collection records that correspond to materials itemized in the [Berg Collection Uncataloged Manuscripts](https://archives.nypl.org/brg/19347) finding aid:
  - **Title**: `Berg collection uncataloged manuscripts`
  - **Subtitle**: enter the creator name in direct order
  - E.g. [`Berg collection uncataloged manuscripts: Julia Alvarez`](https://metadata.nypl.org/collection/127550?section=desc_md#:~:text=Title-,Berg%20collection%20uncataloged%20manuscripts%3A%20Julia%20Alvarez,-Name)

---

### Identifier
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/identifier/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For collection records that correspond to materials itemized in the [Berg Collection Uncataloged Manuscripts](https://archives.nypl.org/brg/19347) finding aid:
  - Enter [Archives EAD ID](/metadata-documentation/metadata/element/identifier/archives-ead/) based on the corresponding reference item record in the [MMS QA](/metadata-documentation/resources/glossary/#mms-qa) [collection](https://qa-metadata.nypl.org/collection/129034) and set it to inherit
  - Enter [Archives Components ID](/metadata-documentation/metadata/element/identifier/archives-components/) in the collection record ****based on the corresponding reference item record in the [MMS QA](/metadata-documentation/resources/glossary/#mms-qa) [collection](https://qa-metadata.nypl.org/collection/129034)

---

### Note
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/note/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For collection records that correspond to materials itemized in the [Berg Collection Uncataloged Manuscripts](https://archives.nypl.org/brg/19347) finding aid:
  - Add a **Note** element with the **Type**: **admin** by copying and pasting the following text:
    `Collection is component of "Berg Collection Uncataloged Manuscripts" (https://archives.nypl.org/brg/19347#archives_component_id) (YYYY-MM-DD INITIALS)`
    - Replace `YYYY-MM-DD` with the date in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format
    - Replace `INITIALS` with your initials (see [MMS Database › Quick Reference › User IDs 🔒](https://github.com/NYPL/metadata-tools/blob/master/_mms-database-and-sql-queries/mms-db_quick-reference.md#user-ids))
    - Set the element to inherit
    - E.g. [`Collection is component of "Berg Collection Uncataloged Manuscripts" (https://archives.nypl.org/brg/19347#c1340739) (2024-02-07 SAA)`](https://metadata.nypl.org/collection/127550?section=desc_md#:~:text=Note-,Collection%20is%20component%20of%20%22Berg%20Collection%20Uncataloged%20Manuscripts%22%20\(https%3A//archives.nypl.org/brg/19347%23c1340739\)%20\(2024%2D02%2D07%20SAA\),-\(admin\))
  - Add a **Note** element with the **Type**: **admin** by copying and pasting the following text:
    `[LAST NAME] MMS QA container for reference: [QA CONTAINER URL] (YYYY-MM-DD INITIALS)`
    - Replace `YYYY-MM-DD` with the date in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format
    - Replace `INITIALS` with your initials (see [MMS Database › Quick Reference › User IDs 🔒](https://github.com/NYPL/metadata-tools/blob/master/_mms-database-and-sql-queries/mms-db_quick-reference.md#user-ids))
    - Set the element to inherit
    - E.g. [`Alvarez MMS QA container for reference: https://qa-metadata.nypl.org/containers/492353 (2024-03-18 SAA)`](https://metadata.nypl.org/collections/127550?section=desc_md#:~:text=Note-,Alvarez%20MMS%20QA%20container%20for%20reference%3A%20https%3A//qa%2Dmetadata.nypl.org/containers/492353%20\(2024%2D03%2D18%20SAA\),-\(admin\))

---

### Location
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/location/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

---

#### Call number / Shelf Locator
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Subelement →](/metadata-documentation/metadata/element/location/#call-number--shelf-locator)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For collection records that correspond to materials itemized in the [Berg Collection Uncataloged Manuscripts](https://archives.nypl.org/brg/19347) finding aid:
  - Enter `Berg Collection Uncataloged Manuscripts, NAME`
  - Replace `NAME` with the author name as it is displayed in the finding aid
  - E.g. [`Berg Collection Uncataloged Manuscripts, Alvarez, Julia`](https://metadata.nypl.org/collection/127550?section=desc_md#:~:text=BRG%2C%20Shelf%20locator%3A-,Berg%20Collection%20Uncataloged%20Manuscripts%2C%20Alvarez%2C%20Julia,-Highlighted%20elements%20are)
- For container and item record that correspond to materials itemized in the [Berg Collection Uncataloged Manuscripts](https://archives.nypl.org/brg/19347) finding aid:
  - Enter `Berg Collection Uncataloged Manuscripts, NAME (BOX/FOLDER)`
  - Replace `NAME` with the author name as it is displayed in the finding aid
  - Replace `BOX/FOLDER` with the box and/or folder as it is displayed in the finding aid
  - E.g. [`Berg Collection Uncataloged Manuscripts, Baez, Joan (b. +PB2)`](https://metadata.nypl.org/items/4902455?section=desc_md#:~:text=BRG%2C%20Shelf%20locator%3A-,Berg%20Collection%20Uncataloged%20Manuscripts%2C%20Baez%2C%20Joan%20\(b.%20%2BPB2\),-Elements%20in%20gray)

---

## See Also

- [Berg Collection (Internal Documentation) 🔒](https://docs.google.com/document/d/1I1Q4Jyz3hGo6u37s4dPPFPlscoP55waHTwyezDfGl3o/edit) for the respective [MSU Liason's 🔒](https://docs.google.com/spreadsheets/d/1P-YDJigon640fTCLP4Ig4-zmzqrX88v5M24ShuxFNVY/edit?gid=0) internal documentation and notes related to the Berg Collection