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
- The **MSS Unit ID** is automatically populated into records when [importing finding aids](/metadata-documentation/workflows/importing/finding-aids/)
- If adding a **MSS Unit ID** manually for a collection or standalone item, it can be located with the following methods:
    - In the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal), the **MSS Unit ID** is the numeric slug of the URL, e.g., [https://archives.nypl.org/the/**21738**](https://archives.nypl.org/the/21738)
    - In the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal), the **MSS Unit ID** can also be found by [viewing the XML for a finding aid](/metadata-documentation/resources/tips-tricks/#view-xml-in-archives-portal)
    - The **MSS Unit ID** can be found within the **&lt;unitid&gt;** tag for a finding aid component that has the collection level **attribute**, e.g., &lt;archdesc **level=&quot;collection&quot;**&gt;&lt;did&gt;&lt;unittitle&gt;Avery Willard photographs&lt;/unittitle&gt;&lt;unitdate type=&quot;inclusive&quot; normal=&quot;1919/1993&quot;&gt;1919-1993&lt;/unitdate&gt;&lt;unitdate type=&quot;bulk&quot; normal=&quot;1940/1970&quot;&gt;1940-1970&lt;/unitdate&gt;&lt;unitid type=&quot;local_call&quot;&gt;*T-Vim 1999-026&lt;/unitid&gt;&lt;unitid type=&quot;local_mss&quot;&gt;**21738**&lt;/unitid&gt;
    - In the [Archives Portal Admin Interface](/metadata-documentation/resources/glossary/#archives-portal-admin-interface), the **MSS Unit ID** can be found as the value of the **identifier (local_mss)** field in records with **/collections/** in the URL ([see example](https://archives.nypl.org/admin/collections/582#:~:text=identifier%20(local_mss),21738))

## Format

<dl>
<dt>Preferred structure</dt>
<dd><tt><span style="background: #ffccff; border: 1px solid #5c5962;">unique numeric identifier</span></tt></dd>
<dt>Example</dt>
<dd><a href="https://metadata.nypl.org/collection/61310?section=desc_md#:~:text=Identifier-,local_mss%3A%2021738,-Identifier"><tt><span style="background: #ffccff; border: 1px solid #5c5962;">61310</span></tt></a></dd>
</dl>

## Inheritance
- Set **MSS Unit ID**s added to collections to be **Inheritable**

## Use With
- [NYPL catalog ID (B-number)](/metadata-documentation/metadata/element/identifier/bnumber/), which is automatically imported into the collection or standalone item record when importing either an EAD or PDF finding aid
- [Other local Identifier (Archives collections id)](/metadata-documentation/metadata/element/identifier/other-local/#archives-collections-id), which is automatically imported into the collection or standalone item record when importing an EAD finding aid

## See Also
- [Linking Between Systems › Archives Portal](/metadata-documentation/workflows/linking/#archives-portal) for an overview of how archives-related identifiers create links between Digital Collections and the Archives Portal
- [Importing Metadata › Importing Finding Aids](/metadata-documentation/workflows/importing/finding-aids/) for the workflow of importing a finding aid into MMS
