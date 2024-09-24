---
layout: page
title: Pforzheimer Collection
permalink: /division/pforzheimer/
parent: By Division
grand_parent: MMS › Metadata
nav_exclude: true
---

# Pforzheimer Collection
{: .no_toc }

Provides guidelines for metadata describing material from the Pforzheimer Collection in the Metadata Management System (MMS)

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Guidelines

---

### Identifier
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/identifier/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For container and item records [imported from EAD-encoded finding aids](/metadata-documentation/workflows/importing/finding-aids/):
    - After updating the [**Location**](#location) element, delete the [**Other local identifier**](/metadata-documentation/metadata/element/identifier/other-local/) that follows the format of one or more alphabetic characters, a space, and three or more numeric characters

---

### Location
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/location/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- For container and item records [imported from EAD-encoded finding aids](/metadata-documentation/workflows/importing/finding-aids/):
  - **Override** the inherited **Location** and ensure the **Location** element is correctly populated
    - **Repository**: `The New York Public Library`
    - **NYPL Division/Collection**: `Pforzheimer Collection`
    - **Call number / Shelf Locator**: construct by combining `Pforz MS` with the value imported into in [**Other local identifier**](/metadata-documentation/metadata/element/identifier/other-local/) that follows the format of one or more alphabetic characters, a space, and three or more numeric characters
      - E.g. the [**Call number**](https://archives.nypl.org/cps/19609#:~:text=Call%20number,Pforz%20MS) for [George Gordon Byron, Lord Byron manuscript material](https://metadata.nypl.org/collection/65511) is imported As `Pforz MS`, but an individual component will also have a value in [**Other local identifier**](/metadata-documentation/metadata/element/identifier/other-local/) such as `B 0149`, so the **Call number / Shelf Locator** for that record should be [Pforz MS (B 0149)](https://metadata.nypl.org/items/5453242?section=desc_md#:~:text=CPS%2C%20Shelf%20locator%3A-,Pforz%20MS%20\(B%200149\),-Elements%20in%20gray)
  - Delete the [**Other local identifier**](/metadata-documentation/metadata/element/identifier/other-local/) after updating the **Location** element

---

## See Also

- [Pforzheimer Collection (Internal Documentation) 🔒](https://docs.google.com/document/d/13TDDGPf0_oPJyaaX3WAMsEI0nsErB64XIEnNX58-yc8/edit) for the respective [MSU Liason's 🔒](https://docs.google.com/spreadsheets/d/1P-YDJigon640fTCLP4Ig4-zmzqrX88v5M24ShuxFNVY/edit?gid=0) internal documentation and notes related to the Pforzheimer Collection