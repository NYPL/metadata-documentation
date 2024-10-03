---
layout: page
title: Linking Between Systems
permalink: /workflows/linking/
parent: MMS › Workflows
nav_order: 8
---

# Linking Between Systems
{: .no_toc }

Provides an overview of the use of [identifiers](/metadata-documentation/metadata/element/identifier/) in the Metadata Management System (MMS) to support connections to and from Digital Collections (DC) from other patron-facing systems of the Library

{: .note }
If a link to or from Digital Collections is absent or broken, please let us know via our [Contact Form](/metadata-documentation/contact/form/) so we can investigate.

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Research Catalog

### Digital Collections → Research Catalog

- When a [bnumber](/metadata-documentation/metadata/element/identifier/bnumber/) is present in MMS for an collection, container, or item, a link to the Research Catalog will automatically appear on that entity's page on DC
    - From a collection or container view, the linked bnumber can be found on the **About** tab in the **Identifiers** section as **NYPL catalog ID (B-number)**
    - From an item view, a link can be found in two places:
        - In the right column titled **View This Item Elsewhere** in a box titled **NYPL Catalog** and **View this item in the NYPL Catalog**
        - Towards the end of the descriptive metadata in the **Identifiers** section as **NYPL catalog ID (B-number)**
    - If more than one bnumber is present on an MMS record, only one link will be linked from the **View This Item Elsewhere** column but every bnumber and its corresponding link will appear in the **Identifiers** section

### Research Catalog → Digital Collections

- When a [bnumber](/metadata-documentation/metadata/element/identifier/bnumber/) is added in MMS to a collection, container, or item that has met the [criteria to appear in DC](/metadata-documentation/dc/criteria/), a link to DC will be added to the corresponding catalog record
    - In the [Research Catalog](/metadata-documentation/resources/glossary/#research-catalog), the link can be found under the **Available Online** heading or the **Connect to:** section as **NYPL Digital Collections**
    - In the [Legacy Catalog](/metadata-documentation/resources/glossary/#legacy-catalog), the link can be found under the **Connect to:** heading as NYPL Digital Collections
    - Links to DC are added to the bibliographic record in Sierra
        - Links to DC should use the standardized MARC 856 field:<br><tt>856 41 |u<span style="background: #ffffcc; border: 1px solid #5c5962;">URL</span>|zNYPL Digital Collections</tt>
    - URLs are formatted according to our [URL Structure](/metadata-documentation/dc/url-structure/) documentation
- Links to DC are periodically batch added to Sierra by the ​​Library's Integrated Library Systems Team (ILS Team) using data supplied by the Metadata Services Unit (MSU)
    - This workflow is still being refined, but our current goal is to supply refreshed data to the Library's ILS Team on a regular basis so they can perform batch updates
    - Past batches of supplied links can be found in the [Data Supplied to ILS Team 🔒](https://drive.google.com/drive/folders/1ktPZqRYoIv0yJIWTwLDeRhM766GKaDU7?usp=sharing) folder in Google Drive
    - Library staff with relevant permissions can access related scripts in our [metadata-tools 🔒](https://github.com/NYPL/metadata-tools/tree/master/_quarterly_bnumber) repo

## Archives Portal

### Digital Collections → Archives Portal

#### Via MSS Unit ID
- When an [MSS Unit ID](/metadata-documentation/metadata/element/identifier/mss-unit/) is present on an MMS collection, container, or item, the **MSS Unit ID** numeric string will automatically appear on that entity's page on DC
    - From a collection or container view, the collection's **MSS Unit ID** numeric string can be found on the **About** tab in the **Identifiers** section as **MSS Unit ID**
    - From an item view, the **MSS Unit ID** numeric string can be found towards the end of the descriptive metadata in the **Identifiers** section as **MSS Unit ID**
- The **MSS Unit ID** identifiers on DC do not link to the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal)
- To navigate to the Archives Portal collection that corresponds to content in Digital Collections, append the MSS Unit ID numeric string to <tt>https://archives.nypl.org/</tt>
<dl>
<dt>URL structure</dt>
<dd><tt>https://archives.nypl.org/<span style="background: #ccccff; border: 1px solid #5c5962;">MSS Unit ID</span></tt></dd>
<dt>URL example</dt>
<dd><tt><a href="https://archives.nypl.org/21423">https://archives.nypl.org/<span style="background: #ccccff; border: 1px solid #5c5962;">21423</span></a></tt></dd>
<dt>Resolved URL structure</dt>
<dd><tt>https://archives.nypl.org/<span style="background: #ffcc99; border: 1px solid #5c5962;">divcode</span>/<span style="background: #ccccff; border: 1px solid #5c5962;">MSS Unit ID</span></tt></dd>
<dt>Resolved URL example</dt>
<dd><tt><a href="https://archives.nypl.org/the/21423">https://archives.nypl.org/<span style="background: #ffcc99; border: 1px solid #5c5962;">the</span>/<span style="background: #ccccff; border: 1px solid #5c5962;">21423</span></a></tt></dd>
</dl>

#### Via Archives EAD ID & Archives Components ID
- When an [Archives EAD ID](/metadata/element/identifier/archives-ead/) is present on an MMS item, the **Archives EAD ID** link will automatically appear on that item's page on DC
    - From an item view, the **Archives EAD ID** link can be found towards the end of the descriptive metadata in the **Identifiers** section as **Archives EAD ID**
    - Clicking the link will take you to the item's finding aid component in the Archives Portal and will resolve to a URL that uses the [Archives Components ID](/metadata-documentation/metadata/element/identifier/archives-components/)

<dl>

<dt>URL structure</dt>
<dd><tt>http://archives.nypl.org/components/<span style="background: #ffccff; border: 1px solid #5c5962;">Archives EAD ID</span></tt></dd>

<dt>URL example</dt>
<dd><tt><a href="http://archives.nypl.org/components/3329690">http://archives.nypl.org/components/<span style="background: #ffccff; border: 1px solid #5c5962;">3329690</span></a></tt></dd>

<dt>Resolved URL structure</dt>
<dd><tt>https://archives.nypl.org/<span style="background: #ffcc99; border: 1px solid #5c5962;">divcode</span>/<span style="background: #ccccff; border: 1px solid #5c5962;">MSS Unit ID</span>#c<span style="background: #ccff99; border: 1px solid #5c5962;">Archives components id</span></tt></dd>

<dt>Resolved URL example</dt>
<dd><tt><a href="https://archives.nypl.org/cps/24637#c1638681">https://archives.nypl.org/<span style="background: #ffcc99; border: 1px solid #5c5962;">cps</span>/<span style="background: #ccccff; border: 1px solid #5c5962;">24637</span>#c<span style="background: #ccff99; border: 1px solid #5c5962;">1638681</span></a></tt></dd>

</dl>

### Archives Portal → Digital Collections
- Digitized assets for records that are [available globally](/metadata-documentation/dc/criteria/) in Digital Collections are displayed in the Archives Portal
    - For EAD-encoded finding aids, an icon and clickable link will be present to the left of the associated finding aid component ([example](https://archives.nypl.org/mss/3306#detailed))
        - This connection is made via the [Archives EAD ID](/metadata-documentation/metadata/element/identifier/archives-ead/)
        - The icon displayed is determined by the type of digitized asset
            - For images, the icon will be a film strip (🎞️)
            - For sound recordings, the icon will be music notes (🎶)
            - For moving images, the icon will be a film camera (📽️)
    - For PDF finding aids, thumbnails will display on the **Overview** tab of the collection ([example](https://archives.nypl.org/dan/23194#:~:text=is%20mostly%20undated.-,DIGITAL%20ASSETS,-1%20Images))
        - This connection is made via the [MSS Unit ID](/metadata-documentation/metadata/element/identifier/mss-unit/)
- Right clicking and opening any icon or thumbnail in a new tab will take the user directly to the corresponding record on Digital Collections