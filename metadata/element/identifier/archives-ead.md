---
layout: page
title: Archives EAD ID
permalink: /metadata/element/identifier/archives-ead/
parent: Identifier
grand_parent: By Element
nav_exclude: true
---

# Archives EAD ID
{: .d-inline .v-align-middle .no_toc .mr-2 }
Required if Applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }

Identifier that correlates [EAD](/metadata-documentation/resources/glossary/#encoded-archival-description)-encoded finding aid components to their MMS container or item records, facilitating the display of digitized assets in the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal)
{: .d-block .mt-2 .fs-6 .fw-300 }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Source
- [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal)

## Guidelines
- **Archives EAD ID**s are automatically imported into their respective MMS container and/or item records when [importing an EAD-encoded finding aid](/metadata-documentation/workflows/importing/finding-aids/) into MMS
- For large and/or complex collections with EAD-encoded finding aids where a sizeable number of records are missing **Archives EAD ID**s, reimporting the finding aid is recommended
    - After reimporting, relocate captures and reassigning rights to ensure all of the archives-related identifiers are correct in MMS
- For smaller or less complex collections, it may be more time effective to manually adding missing **Archives EAD ID**s to the respective container and item records
- If adding a **Archives EAD ID** manually for a container or item, it can be located with the following methods:
    - In the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal), the **Archives EAD ID** can only be found by [viewing the XML for an EAD-encoded finding aid](/metadata-documentation/resources/tips-tricks/#view-xml-in-archives-portal)
    - The **Archives EAD ID** can be found within the **&lt;unitid&gt;** tag for a finding aid component that has the level attribute of **file**, e.g., &lt;c05 **level=&quot;file&quot;**&gt;&lt;did&gt;&lt;unittitle&gt;Playbill, Ethel Barrymore Theatre&lt;/unittitle&gt;&lt;unitdate type=&quot;inclusive&quot; normal=&quot;1965-04&quot;&gt;April 1965&lt;/unitdate&gt;&lt;unitid type=&quot;local_mss&quot;&gt;**1749132**&lt;/unitid&gt;
- In the [Archives Portal Admin Interface](/metadata-documentation/resources/glossary/#archives-portal-admin-interface), the **Archives EAD ID** can be found as the value of the **identifier (local_mss)** field in records with **/components/** in the URL ([see example](https://archives.nypl.org/admin/components/1418303#:~:text=identifier%20(local_mss),1749132))

## Format

<dl>
<dt>Preferred structure</dt>
<dd><tt><span style="background: #ffccff; border: 1px solid #5c5962;">unique numeric identifier</span></tt></dd>
<dt>Example</dt>
<dd><a href="https://metadata.nypl.org/items/5342251?section=desc_md#:~:text=Archives%20EAD%20ID%3A-,1749132,-Identifier"><tt><span style="background: #ffccff; border: 1px solid #5c5962;">1749132</span></tt></a></dd>
</dl>

## Inheritance
- If an item record with an **Archives EAD ID** is converted to a container, set the **Archives EAD ID** to be **Inheritable**

## Use With
- [MSS Unit ID](/metadata-documentation/metadata/element/identifier/mss-unit/), which should always be present through inheritance for a record with an **Archives EAD ID**
- [Other local Identifier (Archives components id)](/metadata-documentation/metadata/element/identifier/other-local/#archives-collections-id), which are automatically imported into container and/or item records alongside **Archives EAD ID**s for collections with EAD-encoded finding aids

## See Also
- [Linking Between Systems › Archives Portal](/metadata-documentation/workflows/linking/#archives-portal) for an overview of how archives-related identifiers create links between Digital Collections and the Archives Portal
- [Importing Metadata › Importing Finding Aids](/metadata-documentation/workflows/importing/finding-aids/) for the workflow of importing a finding aid into MMS