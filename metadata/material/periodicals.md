---
layout: page
title: Periodicals
permalink: /metadata/material/periodicals/
parent: By Material
grand_parent: MMS › Metadata
nav_exclude: true
---

# Periodicals
{: .no_toc }

Provides guidelines for metadata specific to periodicals such as magazines and newspapers described in the Metadata Management System (MMS)

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

- For partially-digitized periodicals, structure an issue of the periodical as a container with a child item for each page or consecutive page range, e.g.:
```
| -- Collection = periodical
   | -- Container = volume
      | -- Container = issue
         | -- Item = page(s)
```
- For fully-digitized periodicals, structure an issue of the periodical as an item with multiple captures, e.g.:
```
| -- Collection = periodical
   | -- Container = volume
      | -- Item = issue
```
- For periodical collections containing a mix of partially- and fully-digitized issues within the same volume, structure using a hybrid approach, e.g.:
```
| -- Collection = periodical
   | -- Container = volume
      | -- Item = issue
   | -- Container = volume
      | -- Container = issue
         | -- Item = page(s)
```
- Reorder containers and items as needed to maintain sequential order

---

### Title
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/title/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For a collection record representing the periodical, use the full periodical title
  - E.g. [`Courrier cinematographique: Organe hebdomadaire indépendent de la cinematographie des arts, sciences et industries qui s'y rattachent`](https://metadata.nypl.org/collection/56910?section=desc_md#titleInfo_0)
- For a container record representing a volume:
  - **Title**: enter the periodical title (may be shortened for long titles)
    - E.g. `Courrier cinematographique`
  - **Part Number**: enter `Volume` followed by the volume number
    - E.g. `Volume 20`
- For an container or item record representing an issue:
  - **Title**: enter the periodical title (may be shortened for long titles)
    - E.g. `Courrier cinematographique`
  - **Part Number**: enter the volume number, issue number, and/or date
    - To indicate the volume number, enter `Volume` followed by the volume number
      - E.g. `Volume 20`
    - To indicate the issue number, enter `Number` followed by the issue number
      - E.g. `Number 26`
    - To indicate the date, enter the month (and/or day) and year; month or season and year; or year alone
      - E.g. `February 1973`
    - Each of these part numbers components can be combined
      - If adding both a volume number and issue number, use a comma as a separator and do not capitalize `number`
        - E.g. `Volume 20, number 26`
      - If adding both volume/issue numbers and a date, enclose the date in parentheses
        - E.g. `Volume 1, number 1 (January/March 1974)`
      - See [MARC 362](https://www.oclc.org/bibformats/en/3xx/362.html) for additional examples
- For an item record representing a portion of a partially-digitized issue:
  - **Title**: enter the periodical title (may be shortened for long titles)
  - **Part Number**: enter the volume, issue, and/or page numbers
    - To indicate the volume number, enter `Volume` followed by the volume number
      - E.g. `Volume 20`
    - To indicate the issue number, enter `Number` followed by the issue number
      - E.g. `Number 26`
    - To indicate the date, enter the month (and/or day) and year; month or season and year; or year alone
      - E.g. `February 1973`
    - To indicate an individual page number, enter `page` followed by the page number and enclose in brackets
      - E.g. `[page 8]`
    - To indicate a consecutive page range, enter `pages` followed by the page range separated by a hyphen and enclose in brackets
      - E.g. `[pages 3-5]`
    - Each of these part numbers components can be combined
      - If adding both a volume number and issue number, use a comma as a separator and do not capitalize `number`
        - E.g. `Volume 20, number 26`
      - If adding both volume/issue numbers and a date, enclose the date in parentheses
        - E.g. `Volume 1, number 1 (January/March 1974)`
      - If adding page numbers, append the page number or range to the rest of the part number components
        - E.g. `Volume 20, number 26 [page 8]` or `Volume 1, number 1 (January/March 1974) [pages 3-5]`
      - See [MARC 362](https://www.oclc.org/bibformats/en/3xx/362.html) for additional examples
  - **Part Name**: enter a descriptive part name if no page numbers are included in **Part Number**, e.g.:
    - For a cover, use `[front cover]` enclosed in brackets
      - E.g. [`Courrier cinematographique Vol. 20, no. 26 [front cover]`](https://metadata.nypl.org/items/5299562?section=desc_md#titleInfo_0)
    - For an article, transcribe the title from the headline without brackets
    - For an image, transcribe the image caption without brackets
    - In cases where there are multiple titles or captions, additional **Title** elements may be added with one title using the **Primary** attribute

---

### Origin Info
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/origin-info/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

---

#### Issuance
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Subelement →](/metadata-documentation/metadata/element/origin-info/#issuance)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For a collection record representing the periodical, select **serial**

---

#### Date
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Subelement →](/metadata-documentation/metadata/element/origin-info/#date)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For **Type**, select **Date issued**
- For a collection record representing the periodical, enter the **Date range** held by the Library based on the source catalog record
  - If the catalog record indigates an open-ended data range (e.g. `1971-`), enter a date in the **Start date** without an **End date**
  - Do not set the **Date range** of a collection record to be **Inheritable**
- For a container record representing a volume, enter the **Date range** that corresponds to that volume
- For an container or item record representing an issue where a specific date is not provided, enter a year or date range with the appropriate **Qualifier**
    - E.g. **inferred** may be used when a possible date range for an issue is inferred from the volume

---

### Genre
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/genre/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- Add **Genre** based on the [Genre (non-AMI) 🔒](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027) tab of the [Genre + Form + Extent 🔒](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit) spreadsheet, which includes:
  - [Periodicals](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027\&range=A232)
  - [Newspapers](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027\&range=A215)
  - [Zines](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027\&range=A362)
- For an item record representing a portion of a partially-digitized issue, add a **Genre** that describes the item, e.g.
  - [Magazine covers](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027\&range=A191)
  - [articles](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027\&range=A19)
  - [Illustrations](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027\&range=A154)

---

### Physical Description
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/physical-description/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For a collection record representing the periodical, do not set the **Physical description** to be **Inheritable**
- For periodicals digitized from a microform (including microfiche and microfilm), add a **Form** subelement with [Microforms](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=500310202\&range=D36) as the value to the appropriate collection- or container record and set to be **Inheritable**

---

### Subject
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/subject/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For a collection record representing the periodical, **Subject** values should represent either all or a signififcant portion of periodical as a whole
  - If appropriate to all child records, a subject can be set to **Inheritable**
- Additional subjects can be added to item records as appropriate

---

### Note
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/note/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For a collection record representing the periodical, a **Note** element should generally not be set to **Inheritable** unless it applies to all child records
- For bound periodicals, add binding information as a **Note** element with the [**Type**](/metadata-documentation/metadata/element/note/#type): **content**
- For periodicals digitized from a microform (including microfiche and microfilm), add a microform details as a **Note** element with the [**Type**](/metadata-documentation/metadata/element/note/#type): **reproduction** and set to be **Inheritable**
    - E.g. `On Reel 46 B (Sept. 1-Dec. 31, 1886)`

---

### Location
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/location/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- Set **Location** at the collection level and set to be **Inheritable**
- [MARC 852$z](https://www.oclc.org/bibformats/en/8xx/852.html#subfieldz) from the original bibliographic record can be omitted