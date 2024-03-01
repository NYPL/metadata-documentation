---
layout: page
title: Archives Components ID
permalink: /metadata/element/identifier/archives-components/
parent: Identifier
grand_parent: By Element
nav_exclude: true
---

# Archives Components ID
{: .d-inline .v-align-middle .no_toc .mr-2 }

Identifier that connects archives components from the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal) and the [Archives Portal Admin Interface](/metadata-documentation/resources/glossary/#archives-portal-admin-interface) to the MMS container or item records, present only for EAD-encoded finding aids
{: .d-block .mt-2 .fs-6 .fw-300 }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Source

- [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal)


## Guidelines

- The **Archives Components ID** is automatically populated into records when [importing EAD-encoded finding aids](/metadata-documentation/workflows/importing/finding-aids/)
- If adding a **Archives Components ID** manually for a container or item, it can be located with the following methods:
    - In the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal), the **Archives Components ID** can be found by [viewing the XML for an EAD-encoded finding aid](/metadata-documentation/resources/tips-tricks/#view-xml-in-archives-portal)
        - The **Archives Components ID** is present as the slug in the **\<dao xlink:href=>** tag URL, e.g., \<dao xlink:type="simple" xlink:href="http\://archives.nypl.org/the/21738#d**448691**">
    - In the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal), the **Archives Components ID** is also found in the in-line anchor to the \<div> of the container or item
        - In Google Chrome, right click the container or item description and select **Inspect** to find the **\<div id>** for the selected text
        - A link to the **Archives Components ID** can be constructed with a c ([https://archives.nypl.org/the/21738#**c**448691](https://archives.nypl.org/the/21738#c448691)) to allow a user to hover over the box/folder/location info to display a thumbnail of the digitized asset
        - A link to the **Archives Components ID** can be constructed with a d ([https://archives.nypl.org/the/21738#**d**448691](https://archives.nypl.org/the/21738#d448691)) to allow a user to view the digitized assets within a lightbox
    - In the [Archives Portal Admin Interface](/metadata-documentation/resources/glossary/#archives-portal-admin-interface), the **Archives Components ID** can be found in records with **/components/** in the URL using the following methods:
        - As the numeric slug of the url, e.g., [https://archives.nypl.org/admin/components/**448691**](https://archives.nypl.org/admin/components/448691)
        - As the value of the the **id** field ([see example](https://archives.nypl.org/admin/components/1418303#:~:text=id,1418303))

## Format

<dl>
<dt>Identifier type</dt>
<dd><tt>Archives Components ID</tt></dd>
<dt>Preferred structure</dt>
<dd><tt>archives_components_<span style="background: #ffccff; border: 1px solid #5c5962;">unique numeric identifier</span></tt></dd>
<dt>Example</dt>
<dd><a href="https://metadata.nypl.org/containers/375214?section=desc_md#:~:text=Other%20local%20Identifier%20(Archives%20components%20id)%3A%20archives_components_448691"><tt>archives_components_<span style="background: #ffccff; border: 1px solid #5c5962;">448691</span></tt></a></dd>
</dl>

## Inheritance
- Do not set **Archives Components IDs** to be **Inheritable**

## Use With
- [Archives EAD ID](/metadata-documentation/metadata/element/identifier/archives-ead/), which are automatically imported into the container and/or item records for collections with EAD-encoded finding aids 

## See Also
- [Linking Between Systems › Archives Portal](/metadata-documentation/workflows/linking/#archives-portal) for an overview of how archives-related identifiers create links between Digital Collections and the Archives Portal
- [Importing Metadata › Importing Finding Aids](/metadata-documentation/workflows/importing/finding-aids/) for the workflow of importing a finding aid into MMS