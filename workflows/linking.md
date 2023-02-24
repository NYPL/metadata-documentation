---
layout: page
title: Linking Between Systems
permalink: /workflows/linking/
parent: MMS › Workflows
nav_order: 6
---

{: .highlight-title }
> 🚧 Under Construction
>
> This page is still being developed. Links to legacy documentation may appear to facilitate our migration process. [Contact us](/metadata-documentation/contact/) with any questions or feedback.

# Linking Between Systems
{: .no_toc }

The use of [identifiers](/metadata-documentation/metadata/element/identifier/) in the Metadata Management System (MMS) supports connections to and from Digital Collections (DC) from other patron-facing systems of the Library

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Research Catalog

### Digital Collections → Research Catalog

- When a [bnumber](/metadata-documentation/metadata/element/identifier/#nypl-catalog-id-b-number) is present on an MMS collection, container, or item, a link to the Research Catalog will automatically appear on that entity's page on DC
    - From a collection or container view, the linked bnumber can be found on the **About** tab in the **Identifiers** section as **NYPL catalog ID (B-number)**
    - From an item view, a link can be found in two places:
        -  In the right column titled **View This Item Elsewhere** in a box titled **NYPL Catalog** and **View this item in the NYPL Catalog**
        - Towards the end of the descriptive metadata in the **Identifiers** section as **NYPL catalog ID (B-number)**
    - If more than one bnumber is present on an MMS record, only one link will be linked from the **View This Item Elsewhere** column but every bnumber and its corresponding link will appear in the **Identifiers** section
- Use our [Metadata Reporting Form](/metadata-documentation/contact/form/) if links from DC to the Research Catalog are absent or broken

### Research Catalog → Digital Collections

- When a [bnumber](/metadata-documentation/metadata/element/identifier/#nypl-catalog-id-b-number) is added in MMS to a collection, container, or item that has met the [criteria to appear in DC](/metadata-documentation/dc/criteria/), a link to DC will be added to the corresponding catalog record
    - In the [Research Catalog](/metadata-documentation/resources/glossary/#research-catalog), the link can be found under the **Available Online** heading or the **Connect to:** section as **NYPL Digital Collections**
    - In the [Legacy Catalog](/metadata-documentation/resources/glossary/#legacy-catalog), the link can be found under the **Connect to:** heading as NYPL Digital Collections
    - Links to DC are added to the bibliographic record in Sierra
        - Links to DC should use the standardized MARC 856 field:<br><tt>856 41 |u<span style="background: #ffffcc; border: 1px solid #5c5962;">URL</span>|zNYPL Digital Collections</tt>
    - URLs are formatted according to our [URL Structure](/metadata-documentation/dc/url-structure/) documentation, and then run through the Library's [Link Minter](/metadata-documentation/resources/glossary/#link-minter) tool
- Links to DC are periodically batch added to Sierra by the ​​Library's Integrated Library Systems Team (ILS Team) using data supplied by the Metadata Services Unit (MSU)
    - This workflow is still being refined, but our current goal is to supply refreshed data to the Library's ILS Team every six months so they can perform batch updates
    - Past batches of supplied links can be found in the [Data Supplied to ILS Team 🔒](https://drive.google.com/drive/folders/1ktPZqRYoIv0yJIWTwLDeRhM766GKaDU7?usp=sharing) folder in Google Drive
    - Library staff with relevant permissions can access related scripts in our [metadata-tools 🔒](https://github.com/NYPL/metadata-tools/tree/master/_quarterly_bnumber) repo
- Use our [Metadata Reporting Form](/metadata-documentation/contact/form/) if links from the Research Catalog to DC are absent or broken

## Archives Portal