---
layout: page
title: Identifier
permalink: /metadata/element/identifier/
parent: By Element
grand_parent: MMS › Metadata
nav_exclude: true
nav_order: 3
---

{: .highlight-title }
> 🚧 Under Construction
>
> This page is still being developed. Links to legacy documentation may appear to facilitate our migration process. [Contact us](/metadata-documentation/contact/) with any questions or feedback.

# Identifiers
{: .d-inline .v-align-middle .no_toc .mr-2 }
Required
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
Repeatable
{: .d-inline .v-align-middle .label .label-green .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/identifier.html)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

A unique standard number or code that distinctively identifies a resource
{: .d-block .mt-2 .fs-6 .fw-300 }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Purpose
- To uniquely identify a resource locally, within a repository or globally
- To point the user to a description of the resource in another database, such as an original catalog record or a finding aid
- To aggregate related resources for a specific purpose, for instance, identifying images displayed in an online exhibition

## Guidelines
- To meet our [minimum metadata requirements](/metadata-documentation/metadata/guidelines/#minimum-metadata-requirements), an item record must have a [**NYPL catalog ID (B-number)**](/metadata-documentation/metadata/element/identifier/bnumber/), [**MSS Unit ID**](/metadata-documentation/metadata/element/identifier/mss-unit/), and/or [**TMS ID**](/metadata-documentation/metadata/element/identifier/tms/)
    - Ensure at least one required identifier exists at the item level:
        - [**NYPL catalog ID (B-number)**](/metadata-documentation/metadata/element/identifier/bnumber/) for material described in [Sierra](/metadata-documentation/resources/glossary/#sierra)
        - [**MSS Unit ID**](/metadata-documentation/metadata/element/identifier/mss-unit/) for material described in the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal)
        - [**TMS ID**](/metadata-documentation/metadata/element/identifier/tms/) for material described in the [Prints and Photographs Online Catalog](/metadata-documentation/resources/glossary/#prints-and-photographs-online-catalog)
    - Required identifiers can either be assigned to the item itself or [inherited](/metadata-documentation/metadata/guidelines/#inheritance) from a collection or container
    - If you are unable to add one of the above required identifiers, discuss with the [Manager, Metadata Services](/metadata-documentation/contact/), before proceeding further
- Additional identifier requirements include:
    - Item records related [Public Orders (POs)](/metadata-documentation/workflows/digitization/po/) must have a [**Photo Order**](/metadata-documentation/metadata/element/identifier/po/) identifier
    - Item records related to [exhibitions](/metadata-documentation/workflows/digitization/exhibitions/) must have a [**NYPL Exhibition ID**](/metadata-documentation/metadata/element/identifier/nypl-exhibition/)
    - Item records for components of collections on the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal) described with [Encoded Archival Description (EAD)](/metadata-documentation/resources/glossary/#encoded-archival-description) must have an [**Archives EAD ID**](/metadata-documentation/metadata/element/identifier/archives-ead/)
- Other identifiers may be added as appropriate
    - See [**Type**](#type) for a complete list
- Refer to the page for the selected identifier [Type](#type) for details on:
    - **Source**: where the identifier value comes from
    - **Guidelines**: how to use the identifier value
    - **Format**: in what format the identifier value should be input
    - **Inheritance**: if and how an identifier's inheritance should be configured
    - **Use With**: other related identifiers that should be used in conjunction with a given identifier

---

## Attributes

---

### Type
{: .d-inline .v-align-middle .mr-2 }
Required
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/identifier.html#type)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_Identifies the type of identifier that is recorded, for example ISBN, ISSN, ISNI_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Select the **Type** of identifier you wish to add from the dropdown menu:

<dl>

<dt><a href="/metadata-documentation/metadata/element/identifier/ami/">AMI Identifier</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/ami-other/">AMI Other ID</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/ami-primary/">AMI Primary Identifier</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/ami-project/">AMI Project</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/archives-ead/">Archives EAD ID</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/barcode/">Barcode</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/catnyp/">CATNYP ID (legacy)</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/cms-collection/">CMS Collection Identifier</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/cms/">CMS Identifier</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/capture-original-filename/">Capture Original Filename</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/digital-gallery-image/">Digital Gallery Image ID</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/electronic-record-package/">Electronic Record Package</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/hades-collection-guide/">Hades Collection Guide ID (legacy)</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/hades-struc/">Hades struc ID (legacy)</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/isan/">International Standard Audiovisual Number</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/isbn/">International Standard Book Number</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/ismn/">International Standard Music Number</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/ismwc/">International Standard Musical Work Code</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/isrc/">International Standard Recording Code</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/issn/">International Standard Serial Number</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/istc/">International Standard Text Code</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/lccn/">Library of Congress Control Number</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/linking-issn/">Linking International Standard Serial Number</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/mss-unit/">MSS Unit ID</a></dt>
<dd>collection-level identifier for an archival collection in the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal)</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/nypl-exhibition/">NYPL Exhibition ID</a></dt>
<dd>identifier for digitized surrogates of material included in exhibitions at the New York Public Library</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/bnumber/">NYPL catalog ID (B-number)</a></dt>
<dd>primary identifier for a bibliographic record in Sierra, where b-number (or “bnumber”) is short for bibliographic number</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/other-local/">Other local Identifier</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/po/">Photo Order</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/preservica/">Preservica ID</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/publishers-music-plate-number/">Publisher's music plate number</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/publisher-assigned-music-number/">Publisher-assigned music number</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/publisher-assigned-videorecording-number/">Publisher-assigned videorecording number</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/rlin-oclc/">RLIN/OCLC</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/serial-item-and-contribution/">Serial Item and Contribution Identifier</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/sound-recording-issue-number/">Sound recording issue number</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/sound-recording-matrix-number/">Sound recording matrix number</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/strn/">Standard Technical Report Number</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/tms/">TMS ID</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/tms-object-number/">TMS Object Number</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/us-national-gazetteer-feature-name-identifier/">U.S. National Gazetteer Feature Name Identifier</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/uniform-resource/">Uniform Resource Identifier</a></dt>
<dd>definition TK</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/uniform-resource-name/">Uniform Resource Name</a></dt>
<dd>definition TK</dd>

</dl>

---

## See Also
- [Top-level Element: &lt;identifier&gt;](https://www.loc.gov/standards/mods/userguide/identifier.html) for official MODS documentation from the Library of Congress
- [Linking Between Systems](/metadata-documentation/workflows/linking/) for an explanation of how identifiers are used to generate links between Library systems