---
layout: page
title: MSS Unit ID
permalink: /metadata/element/identifier/mss-unit/
parent: Identifier
grand_parent: By Element
nav_exclude: true
---

# MSS Unit ID
{: .d-inline .v-align-middle .no_toc .mr-2 }
Required if Applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }

Collection-level identifier for an archival collection in the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal)
{: .d-block .mt-2 .fs-6 .fw-300 }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Source
- [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal)

## Guidelines
- The **MSS Unit ID** is automatically populated into records when [importing finding aids](/metadata-documentation/workflows/import/#importing-finding-aids)
- If adding a **MSS Unit ID** manually for a collection or standalone item, it can be located with the following methods:
    - In the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal), the **MSS Unit ID** is the numeric slug of the url, e.g., <https://archives.nypl.org/scm/24143>
    - In the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal), the **MSS Unit ID** can also be found by [viewing the XML for a finding aid](/metadata-documentation/resources/tips-tricks/#view-xml-in-archives-portal)
    - The **MSS Unit ID** can be found within the **<unitid>** tag for a finding aid component that has the collection level **attribute**, e.g., <archdesc **level="collection"**><did><unittitle>James Baldwin papers</unittitle><unitdate type="inclusive" normal="1936/1992">1936-1992</unitdate><unitid type="local_mss">**24143**</unitid>
    - In the [Archives Portal Admin Interface](/metadata-documentation/resources/glossary/#archives-portal-admin-interface), the **MSS Unit ID** can be found as the value of the **identifier (local_mss)** field in records with **/collections/** in the URL ([see example](https://archives.nypl.org/admin/collections/10793#:~:text=identifier%20(local_mss),24143))

## Format

<dl>
<dt>Preferred structure</dt>
<dd><tt><span style="background: #ffccff; border: 1px solid #5c5962;">unique numeric identifier</span></tt></dd>
<dt>Example</dt>
<dd><a href="https://archives.nypl.org/scm/24143"><tt><span style="background: #ffccff; border: 1px solid #5c5962;">24143</span></tt></a></dd>
</dl>

## Inheritance
- Set **MSS Unit ID** s added to collections to be **Inheritable**

## Use With
- [NYPL catalog ID (B-number)](/metadata-documentation/metadata/element/identifier/bnumber/), which is automatically imported into the collection or standalone item record when importing either an EAD or PDF finding aid
- [Other local Identifier (Archives collections id)](/metadata-documentation/metadata/element/identifier/other-local/#archives-collections-id), which is automatically imported into the collection or standalone item record when importing an EAD finding aid

## See Also
- [Linking Between Systems › Archives Portal](/metadata-documentation/workflows/linking/#archives-portal) for an overview of how archives-related identifiers create links between Digital Collections and the Archives Portal
- [Importing Metadata › Importing Finding Aids](/metadata-documentation/workflows/import/#importing-finding-aids) for the workflow of importing a finding aid into MMS