---
layout: page
title: Other local Identifier
permalink: /metadata/element/identifier/other-local/
parent: Identifier
grand_parent: By Element
nav_exclude: true
---

# Other local Identifier
{: .d-inline .v-align-middle .no_toc .mr-2 }

Free-text identifier field that can contain any value, used when adding an identifier that does not align with any predefined Identifier type in the Metadata Management System (MMS)
{: .d-block .mt-2 .fs-6 .fw-300 }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Guidelines
- When selecting **Other local Identifier** from the identifier drop-down menu, an additional **Specify identifier type** field will be available
- Adding a value in the  **Specify identifier type** field is strongly recommended
    - If left blank, the value of the **Specify identifier type** field will automatically update to “Other local Identifier” once the record is saved
- The **Other local Identifier** field may be used in standardized ways for common identifiers, see the subheadings below
    - For specific projects (e.g. [Emmet numbers](https://metadata.nypl.org/items/6072588?section=desc_md#:~:text=Other%20local%20Identifier%20\(Emmet%20number\)%3A%20EM.%207337) for the [Thomas Addis Emmet collection](https://metadata.nypl.org/collection/75813)), follow the guidelines provided by the division 

---

### Archives Collections ID
_Identifier that connects an archives collection from the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal) and the [Archives Portal Admin Interface](/metadata-documentation/resources/glossary/#archives-portal-admin-interface) to the MMS collection or standalone item record, present only for EAD-encoded finding aids_

#### Source
- [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal)

#### Guidelines
- The **Archives collections id** is automatically populated into records when [importing finding aids](/metadata-documentation/workflows/import/#importing-finding-aids)
- If adding a **Archives collections id** manually for a collection or standalone item, it can be located in the [Archives Portal Admin Interface](/metadata-documentation/resources/glossary/#archives-portal-admin-interface)
    - As the numeric slug of the URL in records with **/collections/** in the URL, e.g., [https://archives.nypl.org/admin/collections/**10793**](https://archives.nypl.org/admin/collections/10793)
    - As the value of the **id** field ([see example](https://archives.nypl.org/admin/collections/10793#:~:text=id,10793))

#### Format

<dl>
<dt>Identifier type</dt>
<dd><tt>Archives collections id</tt></dd>
<dt>Preferred structure</dt>
<dd><tt>archives_collections_<span style="background: #ffccff; border: 1px solid #5c5962;">unique numeric identifier</span></tt></dd>
<dt>Example</dt>
<dd><a href="https://metadata.nypl.org/collection/59637?section=desc_md#:~:text=Other%20local%20Identifier%20(Archives%20collections%20id)%3A%20archives_collections_24143"><tt>archives_collections_<span style="background: #ffccff; border: 1px solid #5c5962;">10793</span></tt></a></dd>
</dl>

#### Inheritance
- Do not set **Archives collections ids** to be **Inheritable**

#### Use With
- [NYPL catalog ID (B-number)](/metadata-documentation/metadata/element/identifier/bnumber/), which is automatically imported into the collection or standalone item record when importing either an EAD or PDF finding aid
- [MSS Unit ID](/metadata-documentation/metadata/element/identifier/mss-unit/), which is automatically imported into the collection or standalone item record when importing either an EAD or PDF finding aid

#### See Also
- [Linking Between Systems › Archives Portal](/metadata-documentation/workflows/linking/#archives-portal) for an overview of how archives-related identifiers create links between Digital Collections and the Archives Portal
- [Importing Metadata › Importing Finding Aids](/metadata-documentation/workflows/import/#importing-finding-aids) for the workflow of importing a finding aid into MMS

---

### Archives Components ID
_Identifier that connects archives components from the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal) and the [Archives Portal Admin Interface](/metadata-documentation/resources/glossary/#archives-portal-admin-interface) to the MMS container or item records, present only for EAD-encoded finding aids_

#### Source

- [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal)


#### Guidelines

- The **Archives components id** is automatically populated into records when [importing EAD-encoded finding aids](/metadata-documentation/workflows/import/#importing-finding-aids)
- If adding a **Archives components id** manually for a container or item, it can be located with the following methods:
    - In the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal), the **Archives components id** can be found by [viewing the XML for an EAD-encoded finding aid](/metadata-documentation/resources/tips-tricks/#view-xml-in-archives-portal)
        - The **Archives components id** is present as the slug in the **\<dao xlink:href=>** tag URL, e.g., \<dao xlink:type="simple" xlink:href="http\://archives.nypl.org/scm/24143#d**1418303**">
    - In the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal), the **Archives components id** is also found in the in-line anchor to the \<div> of the container or item
        - In Google Chrome, right click the container or item description and select **Inspect** to find the **\<div id>** for the selected text
        - A link to the **Archives components id** can be constructed with a c ([https://archives.nypl.org/scm/24143#**c**1418303](https://archives.nypl.org/scm/24143#c1418303)) to allow a user to hover over the box/folder/location info to display a thumbnail of the digitized asset
        - A link to the **Archives components id** can be constructed with a d ([https://archives.nypl.org/scm/24143#**d**1418303](https://archives.nypl.org/scm/24143#d1418303)) to allow a user to view the digitized assets within a lightbox
    - In the [Archives Portal Admin Interface](/metadata-documentation/resources/glossary/#archives-portal-admin-interface), the **Archives components id** can be found in records with **/components/** in the URL using the following methods:
        - As the numeric slug of the url, e.g., [https://archives.nypl.org/admin/components/**1418303**](https://archives.nypl.org/admin/components/1418303)
        - As the value of the the **id** field ([see example](https://archives.nypl.org/admin/components/1418303#:~:text=id,1418303))

#### Format

<dl>
<dt>Identifier type</dt>
<dd><tt>Archives components id</tt></dd>
<dt>Preferred structure</dt>
<dd><tt>archives_components_<span style="background: #ffccff; border: 1px solid #5c5962;">unique numeric identifier</span></tt></dd>
<dt>Example</dt>
<dd><a href="https://metadata.nypl.org/items/5342251?section=desc_md#:~:text=Other%20local%20Identifier%20(Archives%20components%20id)%3A%20archives_components_1418303"><tt>archives_components_<span style="background: #ffccff; border: 1px solid #5c5962;">1418303</span></tt></a></dd>
</dl>

#### Inheritance
- Do not set **Archives components ids** to be **Inheritable**

#### Use With
- [Archives EAD ID](/metadata-documentation/metadata/element/identifier/archives-ead/), which are automatically imported into the container and/or item records for collections with EAD-encoded finding aids 

#### See Also
- [Linking Between Systems › Archives Portal](/metadata-documentation/workflows/linking/#archives-portal) for an overview of how archives-related identifiers create links between Digital Collections and the Archives Portal
- [Importing Metadata › Importing Finding Aids](/metadata-documentation/workflows/import/#importing-finding-aids) for the workflow of importing a finding aid into MMS