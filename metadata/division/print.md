---
layout: page
title: Print Collection
permalink: /division/print/
parent: By Division
grand_parent: MMS › Metadata
nav_exclude: true
---

# Print Collection
{: .no_toc }

Provides guidelines for metadata describing material from the Print Collection in the Metadata Management System (MMS)

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

- For individual prints that are part of a larger collection (e.g., [Italian master prints](https://metadata.nypl.org/collection/41919)), structure the larger collection as a collection record with a child item for each print:
```
    | -- Collection = larger collection
        | -- Item = print
```
- For prints from a series that are part of a larger collection (e.g. [Jeu de la Mythologie](https://metadata.nypl.org/containers/347813)), structure the larger collection as a collection record, a container record for the series, and a child item within the container for each print:
```
    | -- Collection = larger collection
        | -- Container = series
            | -- Item = print
```
- For prints from a series that are not part of a larger collection, either:
  - Structure a collection record for the series and a child item within the collection for each print (e.g. [Paradise Lost by John Milton: A series of twelve illustrations](https://metadata.nypl.org/collection/29762)):
```
    | -- Collection = primary creator
        | -- Item = print
```
  - Structure a collection record for the primary creator, a container record for the series, and a child item within the container for each print (e.g. [Quelques aspects de la vie de Paris](https://metadata.nypl.org/containers/301831)):
```
    | -- Collection = primary creator
        | -- Container = series
            | -- Item = print
```
- For individual prints that are not part of a larger collection or series (e.g. [Dancer](https://metadata.nypl.org/items/3371530)), structure a collection record for the primary creator with a child item for each print:
```
    | -- Collection = primary creator
        | -- Item = print
```

---

### Title
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/title/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For a collection- or container record representing a series, use the title of the series as the **Title**
- For a collection record containing works by a single creator, use one of the following formats for the **Title**, replacing `[creator]` with the name of creator:
  - `Prints by [creator]`
  - `[Creator]: prints`
  - `[Creator] prints`
- For a item record representing a print:
  - Use the title of the print as the **Title**
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

- Replace [**TMS Object Number**](/metadata-documentation/metadata/element/identifier/tms-object-number/) identifiers with the classmark provided by the division in the **Call number / Shelf Locator** subelement
  - This subelement is populated with the [**TMS Object Number**](/metadata-documentation/metadata/element/identifier/tms-object-number/) automatically when [importing TMS records](/metadata-documentation/workflows/importing/tms/)
  - The Print Collection exclusively uses classmarks to locate items

---

## See Also
- [Wallach Division: Print Collection (Internal Documentation) 🔒](https://docs.google.com/document/d/1HSGFwkRD52qnWlLcmcS-eFvOyb1Jay-kcyZ0PawIAD4/edit) for the respective [MSU Liason’s 🔒](https://docs.google.com/spreadsheets/d/1P-YDJigon640fTCLP4Ig4-zmzqrX88v5M24ShuxFNVY/edit?gid=0) internal documentation and notes related to the Print Collection
- [Importing TMS Records](/metadata-documentation/workflows/importing/tms/) for the workflow to create records in the Metadata Management System (MMS) by importing metadata from records cataloged in The Museum System (TMS)