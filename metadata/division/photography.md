---
layout: page
title: Photography Collection
permalink: /division/photography/
parent: By Division
grand_parent: MMS › Metadata
nav_exclude: true
---

# Photography Collection
{: .no_toc }

Provides guidelines for metadata describing material from the Photography Collection in the Metadata Management System (MMS)

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

{: .note }
> Collection or series titles are typically indicated by the presence of an **Alternate Titles** in the source record.

- For individual photographs that are part of a larger collection (e.g., [Photographs concerning labor, housing and social conditions in the United States](https://metadata.nypl.org/collection/39812)), structure the larger collection as a collection record with a child item for each photograph:
```
    | -- Collection = larger collection
        | -- Item = photograph
```
- For photographs from a series that are part of a larger collection (e.g. [United States](https://metadata.nypl.org/containers/193126?section=overview)), structure the larger collection as a collection record, a container record for the series, and a child item within the container for each photograph:
```
    | -- Collection = larger collection
        | -- Container = series
            | -- Item = photograph
```
- For photographs from a series that are not part of a larger collection, either:
  - Structure a collection record for the series and a child item within the collection for each photograph (e.g. [Particular Voices: Portraits of Gay and Lesbian Writers by Robert Giard](https://metadata.nypl.org/collection/29937)):
```
    | -- Collection = primary creator
        | -- Item = photograph
```
  - Structure a collection record for the primary creator, a container record for the series, and a child item within the container for each photograph (e.g. [Bus Trips to Boston](https://metadata.nypl.org/containers/299588)):
```
    | -- Collection = primary creator
        | -- Container = series
            | -- Item = photograph
```
- For individual photographs that are not part of a larger collection or series (e.g. [Woman on the boardwalk, Coney Island, N.Y.](https://metadata.nypl.org/items/4628918)), structure a collection record for the primary creator with a child item for each photograph:
```
    | -- Collection = primary creator
        | -- Item = photograph
```

---

### Title
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/title/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For a collection- or container record representing a series, use the title of the series as the **Title**
- For a collection record containing works by a single creator, use one of the following formats for the **Title**, replacing `[creator]` with the name of creator:
  - `Photographs by [creator]`
  - `[Creator]: photographs`
  - `[Creator] photographs`
- For a item record representing a photograph:
  - Use the title of the photograph as the **Title**
  - Delete any **Title** elements that correspond to the series after ensuring the item record is located within a collection or container for the series

---

### Name
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/name/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- Adjust **Name** elements to conform to [**Name Part**](/metadata-documentation/metadata/element/name/#name-part) guidelines
- Where a collection or container record containing works by a single creator:
  - Add the **Name** at the highest level appropriate and set it to inherit
  - Remove duplicate **Name** elements from child records
- Delete **Name** elements for anonymous creators (`Anonymous`) unless requested by the division
  - Ensure `Anonymous` are instead included in a [**Note**](https://docs.google.com/document/d/1729J2drDizJ3juW-RH3KIewgNvKLBo85o6nn82pjPMA/edit#note) element with the **Type**: **statement of responsibility**

---

### Note
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/note/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- If the creator is anonymous, add a [**Note**](https://docs.google.com/document/d/1729J2drDizJ3juW-RH3KIewgNvKLBo85o6nn82pjPMA/edit#note) element containing `Anonymous` with the **Type**: **statement of responsibility**

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

- The **Call number / Shelf Locator** should contain the [**TMS Object Number**](/metadata-documentation/metadata/element/identifier/tms-object-number/)
  - This subelement is populated automatically when [importing TMS records](/metadata-documentation/workflows/importing/tms/)
  - It is used by the Photography Collection to locate items

---

## See Also
- [Wallach Division: Photography Collection (Internal Documentation) 🔒](https://docs.google.com/document/d/1Kt90vsEINm0jgRXquCOXRpsSWvZM7ASE6ugFs7-ukNo/edit) for the respective [MSU Liason's 🔒](https://docs.google.com/spreadsheets/d/1P-YDJigon640fTCLP4Ig4-zmzqrX88v5M24ShuxFNVY/edit?gid=0) internal documentation and notes related to the Photography Collection
- [Importing TMS Records](/metadata-documentation/workflows/importing/tms/) for the workflow to create records in the Metadata Management System (MMS) by importing metadata from records cataloged in The Museum System (TMS)
- [Prints and Photographs Discovery](https://ppd.nypl.org/) for source data about items in the Photography Collection