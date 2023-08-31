---
layout: page
title: Electronic Record Package
permalink: /metadata/element/identifier/er/
parent: Identifier
grand_parent: By Element
nav_exclude: true
---

# Electronic Record Package
{: .d-inline .v-align-middle .no_toc .mr-2 }

Number that corresponds to a container of born-digital material described in a finding aid
{: .d-block .mt-2 .fs-6 .fw-300 }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Source
- Assigned by archivist during processing of born-digital material (see [Archivist Workstation Processing Instructions](https://nypl.github.io/digarch/staging/Archivist-Workstation-Processing.html))

## Guidelines
- **Electronic Record Package** identifiers are automatically imported into their respective MMS container and/or item records when [importing an EAD-encoded finding aid](/metadata-documentation/workflows/import/#importing-finding-aids) into MMS
- For large and/or complex collections with EAD-encoded finding aids where a sizeable number of records are missing **Electronic Record Package** identifiers, reimporting the finding aid is recommended
    - After reimporting, relocate captures and request reassignment of rights to ensure all of the archives-related identifiers are correct in MMS
- For smaller or less complex collections, it may be more time effective to manually adding missing **Electronic Record Package** identifiers to the respective container and item records
- If adding a **Electronic Record Package** identifier manually for a container or item, it can be located with the following methods:
    - In the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal), the **Electronic Record Package** identifier can be found on the **Detailed Description** tab to the left of an item or container's title ([see example](https://archives.nypl.org/dan/23068#c1329153))
    - In the [Archives Portal Admin Interface](/metadata-documentation/resources/glossary/#archives-portal-admin-interface), the **Electronic Record Package** identifier can be found in the unitid field with the `"type"=>"local_mss_er"` in records with `/components/` in the URL ([see example](https://archives.nypl.org/admin/components/1329153#:~:text=%7B%22value%22%3D%3E%22er.2%22%2C%20%22type%22%3D%3E%22local_mss_er%22%7D))

## Format

<dl>
<dt>Preferred structure</dt>
<dd><tt>er.<span style="background: #ffccff; border: 1px solid #5c5962;">unique numeric identifier</span></tt></dd>
<dt>Example</dt>
<dd><a href="https://metadata.nypl.org/containers/330553?section=desc_md#:~:text=Electronic%20Record%20Package%3A-,er.2,-Identifier"><tt>er.<span style="background: #ffccff; border: 1px solid #5c5962;">2</span></tt></a></dd>

</dl>

## Inheritance
- If an item record with an **Electronic Record Package** identifier is converted to a container, set the **Electronic Record Package** to be **Inheritable**

## Use With
- [Archives EAD ID](/metadata-documentation/metadata/element/identifier/archives-ead/), which correlates [EAD](/metadata-documentation/resources/glossary/#encoded-archival-description)-encoded finding aid components to their MMS container or item records, facilitating the display of digitized assets in the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal)

## See Also
- [Archivist Workstation Processing Instructions](https://nypl.github.io/digarch/staging/Archivist-Workstation-Processing.html) for documentation from the Library's Digital Archives department describing the workflow where archivists prepare description of born-digital material for a finding aid