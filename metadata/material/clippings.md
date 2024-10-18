---
layout: page
title: Clippings
permalink: /metadata/material/clippings/
parent: By Material
grand_parent: MMS › Metadata
nav_exclude: true
---

# Clippings
{: .no_toc }

Provides guidelines for metadata specific to [clippings](https://dictionary.archivists.org/entry/clipping.html) described in the Metadata Management System (MMS)

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

- Clippings may be structured as:
  - A [standalone item](/metadata-documentation/metadata/record-type/#standalone-item) with multiple captures:\
```
    | -- Item = aggregation of clippings such as a clippings file, scrapbook, or archival collection
        | -- Capture = full sheet
        | -- Capture = full sheet
        | -- Capture = full sheet`
```
    - E.g., [Fancy costumes: scrapbook, approximately 1920-1932](https://metadata.nypl.org/items/4977814)
    - Item record should contain metadata for the item as a whole, not its individual components
  - A collection record with multiple item records:\
```
    | -- Collection = aggregation of clippings such as a clippings file, scrapbook, or archival collection`
        | -- Item = full sheet
            | -- Capture = full sheet
        | -- Item = full sheet
            | -- Capture = full sheet
        | -- Item = full sheet
            | -- Capture = full sheet
```
- E.g., [George Brashear scrapbooks](https://metadata.nypl.org/collection/126590)
- Item record(s) should contain metadata for the item as a whole, not its individual components
- A collection with multiple items, each having multiple captures
```
    | -- Collection = aggregation of clippings such as a clippings file, scrapbook, or archival collection`
        | -- Item = full sheet
            | -- Capture = full sheet
            | -- Capture = detail view
            | -- Capture = detail view
        | -- Item = full sheet
            | -- Capture = full sheet
            | -- Capture = detail view
        | -- Item = full sheet
            | -- Capture = full sheet
            | -- Capture = detail view
            | -- Capture = detail view
            | -- Capture = detail view
```
- E.g., [Alexander Anderson scrapbooks](http://metadata.nypl.org/collection/25829)
- Item record(s) should contain metadata for the individual item, not its parent collection or container

---

### Title
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/title/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For an item, container, or collection record representing an aggregation of clippings such as a clippings file, scrapbook, or archival collection:
  - Add a **Title** element for the aggregation as a whole
    - E.g., [The Billy Rose Theatre Collection clipping file](https://metadata.nypl.org/containers/268759)
- For an item record where only one clipping is visible:
  - Transcribe the **Title** from the clipping’s title, headline, byline, or image caption as appropriate to the clipping
- For an item record with multiple clippings, either:
  - Transcribe each title, headline, byline, or image caption into a single **Title** element separated by `;`
  - Add a separate **Title** element for each clipping containing the respective title, headline, byline, or image caption and check **Primary** for one **Title** element
- See [DCRM(G): Descriptive Cataloging of Rare Materials (Graphics)](https://rbms.info/dcrm/dcrmg/) (“1. Title and Statement of Responsibility Area”) for additional guidelines and examples

---

### Identifier
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/identifier/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

---

### Type of Resource
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/type-of-resource/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

---

### Origin Info
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/origin-info/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

---

#### Date
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Subelement →](/metadata-documentation/metadata/element/origin-info/#date)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For records that include multiple clippings spanning multiple dates, either:
  - Add a **Date range** to describe the range of dates
    - Optionally, in addition to adding a **Date range**, add a [**Note**](/metadata-documentation/metadata/element/note/) with the [**Type**](/metadata-documentation/metadata/element/note/#type): **date** to provide the date of each clipping
  - Add a **Single date** for each clipping

---

#### Place
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Subelement →](/metadata-documentation/metadata/element/origin-info/#place)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For collection records, add a **Place** only when when it applies to the collection as a whole
  - E.g., a scrapbook compiled in New York could have a **Place** value that is set to be **Inheritable**

---

#### Publisher
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Subelement →](/metadata-documentation/metadata/element/origin-info/#publisher)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For collection records, add a **Publisher** only when when it applies to the collection as a whole
  - E.g., a collection of clippings from a single periodical could have a **Publisher** value that is set to be **Inheritable**

---

#### Date
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Subelement →](/metadata-documentation/metadata/element/origin-info/#date)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

---

### Name
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/name/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For a single clipping or where multiple clippings are by the same author:
  - Add single name element
- For multiple clippings each with a different author:
  - Add name element for each author
  - Use **Table of Contents** to specify author for each respective title, headline, byline, and image caption
    - E.g. [`Rev. Joseph Benson, Late Editor of the Methodist Magazine / Jackson Pinxt. ; Holl Sculpt. -- Rev. Joseph Benson / drawing by J. Jackson, R.A., ; engraving by E. Mackenzie`](https://metadata.nypl.org/items/3102112?section=desc_md#:~:text=to%20a%20sheet.-,Table%20of%20Contents,Benson%20/%20drawing%20by%20J.%20Jackson%2C%20R.A.%2C%20%3B%20engraving%20by%20E.%20Mackenzie,-Subject)

---

### Genre
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/genre/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For an collection or container record representing an aggregation of clippings, add [Clippings](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027) as a **Genre** and set to be **Inheritable**
- For an collection or container record representing a scrapbook, add [Scrapbooks](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027\&range=F289) as a **Genre** and do not set to be **Inheritable**
- For an item record representing a single clipping, add [Clippings](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027) as a **Genre** and add additional **Genre** terms as appropriate based on the [Genre (non-AMI) 🔒](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027) tab of the [Genre + Form + Extent 🔒](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit) spreadsheet, which includes:
  - [articles](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027\&range=A19)
  - [Caricatures](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027\&range=A53)
  - [Illustrations](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027\&range=A154)
  - [Magazine covers](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027\&range=A191)
  - [Photographs](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027\&range=A236)
  - [Portraits](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027\&range=A247)
  - [Prints](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027\&range=A256)
  - [Title pages](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027\&range=A333)

---

### Note
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/note/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For item records, **Note** elements can be added with the appropriate **Type** to further describe the clipping
  - For the source of clipping, use **Type**: **content**
    - E.g., `Published in: The daily graphic, September 23, 1886, page 73, as per Google books, viewed April 10, 2017.`