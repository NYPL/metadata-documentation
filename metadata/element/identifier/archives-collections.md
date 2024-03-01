---
layout: page
title: Archives Collections ID
permalink: /metadata/element/identifier/archives-collections/
parent: Identifier
grand_parent: By Element
nav_exclude: true
---

# Archives Collections ID
{: .d-inline .v-align-middle .no_toc .mr-2 }

Identifier that connects an archives collection from the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal) and the [Archives Portal Admin Interface](/metadata-documentation/resources/glossary/#archives-portal-admin-interface) to the MMS collection or standalone item record, present only for EAD-encoded finding aids
{: .d-block .mt-2 .fs-6 .fw-300 }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Source
- [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal)

## Guidelines

{: .warning-title }
> Known Issue
>
> [**MSS Unit ID**](/metadata-documentation/metadata/element/identifier/mss-unit/) is currently being erroneously imported as the **Archives Collections ID** value when [importing a finding aid](/metadata-documentation/workflows/importing/finding-aids/). 
> <small><br>Last checked February 2024</small>

- The **Archives Collections ID** is automatically populated into records when [importing finding aids](/metadata-documentation/workflows/importing/finding-aids/)
- If adding a **Archives Collections ID** manually for a collection or standalone item, it can be located in the [Archives Portal Admin Interface](/metadata-documentation/resources/glossary/#archives-portal-admin-interface)
    - As the numeric slug of the URL in records with **/collections/** in the URL, e.g., [https://archives.nypl.org/admin/collections/**582**](https://archives.nypl.org/admin/collections/582)
    - As the value of the **id** field ([see example](https://archives.nypl.org/admin/collections/582#:~:text=id-,582,-origination))

## Format

<dl>
<dt>Identifier type</dt>
<dd><tt>Archives Collections ID</tt></dd>
<dt>Preferred structure</dt>
<dd><tt>archives_collections_<span style="background: #ffccff; border: 1px solid #5c5962;">unique numeric identifier</span></tt></dd>
<dt>Example</dt>
<dd><a href="https://metadata.nypl.org/collections/61310?section=desc_md#:~:text=Other%20local%20Identifier%20(Archives%20collections%20id)%3A%20archives_collections_582"><tt>archives_collections_<span style="background: #ffccff; border: 1px solid #5c5962;">582</span></tt></a></dd>
</dl>

## Inheritance
- Do not set the **Archives Collections ID** to be **Inheritable**

## Use With
- [NYPL catalog ID (B-number)](/metadata-documentation/metadata/element/identifier/bnumber/), which is automatically imported into the collection or standalone item record when importing either an EAD or PDF finding aid
- [MSS Unit ID](/metadata-documentation/metadata/element/identifier/mss-unit/), which is automatically imported into the collection or standalone item record when importing either an EAD or PDF finding aid

## See Also
- [Linking Between Systems › Archives Portal](/metadata-documentation/workflows/linking/#archives-portal) for an overview of how archives-related identifiers create links between Digital Collections and the Archives Portal
- [Importing Metadata › Importing Finding Aids](/metadata-documentation/workflows/importing/finding-aids/) for the workflow of importing a finding aid into MMS