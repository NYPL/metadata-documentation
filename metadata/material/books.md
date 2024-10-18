---
layout: page
title: Books
permalink: /metadata/material/books/
parent: By Material
grand_parent: MMS › Metadata
nav_exclude: true
---

# Books
{: .no_toc }

Provides guidelines for metadata specific to books described in the Metadata Management System (MMS)

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

- For partially-digitized books, structure the book as a collection with a child item for each page or consecutive page range:
```
    | -- Collection = book
       | -- Item = page(s)
```
- For multi-volume works where a volume is fully-digitized, structure the multi-volume work as a collection with a child item for each volume:
```
    | -- Collection = multi-volume book
       | -- Item = individual volume
```
- For multi-volume containing a mix of partially- and fully-digitized volumes, structure using a hybrid approach:
```
    | -- Collection = multi-volume book
       | -- Item = individual volume
       | -- Container = individual volume
          | -- Item = page(s)
```
- Reorder containers and items as needed to maintain sequential order

---

### Title
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/title/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For a collection, container, or item record representing a full book:
  - **Title**: enter the book title
- For a container or item record representing a volume in a multi-volume work:
  - **Title**: enter the book title (may be shortened for long titles)
  - **Part Number**: enter `Volume` followed by the volume number
    - E.g. [`Volume 3`](https://metadata.nypl.org/items/6392284?section=desc_md)
- For a container or item record representing a specific copy:
  - **Title**: enter the book title (may be shortened for long titles)
  - **Part Number**: enter `copy` followed by the copy number and enclose in brackets
    - E.g. [`[copy 1]`](https://metadata.nypl.org/containers/479513?section=desc_md)
- For an item record representing a portion of a partially-digitized book:
  - **Title**: enter the book title (may be shortened for long titles)
  - **Part Number**: enter the volume, issue, and/or page numbers
    - To indicate the volume number, enter Volume followed by the volume number
      - E.g. `Volume 20`
    - To indicate the copy number, enter `copy` followed by the issue number and enclose in brackets
      - E.g. `[copy 2]`
    - To indicate an individual page number, enter `page` followed by the page number and enclose in brackets
      - E.g. `[page 8]`
    - To indicate a consecutive page range, enter `pages` followed by the page range separated by a hyphen and enclose in brackets
      - E.g. `[pages 3-5]`
    - Each of these part numbers components can be combined
      - If adding both a volume number and copy number, use a comma as a separator and do not capitalize `copy`
        - E.g. `Volume 20 [copy 1]`
      - If adding page numbers, append the page number or range to the rest of the part number components
        - E.g. `Volume 20 [copy 1, page 8]`
  - **Part Name**: enter a descriptive part name if no page numbers are included in **Part Number**, e.g.:
    - For a cover, use `[front cover]` enclosed in brackets
      - E.g. [`[front cover]`](https://metadata.nypl.org/items/5992196?section=desc_md)
    - For an book section or chapter, transcribe the title from the section or title without brackets
    - For an image, transcribe the image caption without brackets
    - In cases where there are multiple titles or captions, additional **Title** elements may be added with one title using the **Primary** attribute

---

### Genre
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/genre/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- Add **Genre** based on the [Genre (non-AMI) 🔒](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027) tab of the [Genre + Form + Extent 🔒](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit) spreadsheet, which includes [Books](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027) and additional narrower terms
- For an item record representing a portion of a partially-digitized book, add a **Genre** that describes the item, e.g.
  - [Title pages](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027\&range=A333)
  - [Frontispieces](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit?gid=1262013027#gid=1262013027\&range=A131)
  - [pages (components)](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027\&range=A224)
  - [folios (leaves)](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027\&range=A129)
  - [articles](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027\&range=A19)
  - [Illustrations](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027\&range=A154)

---

### Note
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/note/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- If there is a **Note** element with the **Type**: **statement of responsibility**:
  - Add a [**Name**](/metadata-documentation/metadata/element/name/) element to the record for any named entities
  - If the **Note** element does not provide additional insight into the role or nature of the attribution besides a named entity represented in a **Name** element, the **Note** element may be removed at the metadata creator's discretion