---
layout: page
title: Identifier
permalink: /metadata/element/identifier/
parent: By Element
grand_parent: MMS › Metadata
nav_exclude: true
nav_order: 3
---

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
<dd>unique identifier of an audio or moving image item assigned during inventory in SPEC</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/ami-other/">AMI Other ID</a></dt>
<dd>free-text identifier field that can contain any value, used when adding an identifier that does not align with any predefined identifier in SPEC for AMI</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/ami-primary/">AMI Primary Identifier</a></dt>
<dd>unique identifier of an audio or moving image item assigned during inventory in SPEC</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/ami-project/">AMI Project</a></dt>
<dd>name of the project under which the media original was digitized</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/archives-collections/">Archives Collections ID</a></dt>
<dd>identifier that connects an archives collection from the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal) and the [Archives Portal Admin Interface](/metadata-documentation/resources/glossary/#archives-portal-admin-interface) to the MMS collection or standalone item record, present only for EAD-encoded finding aids</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/archives-components/">Archives Components ID</a></dt>
<dd>identifier that connects archives components from the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal) and the [Archives Portal Admin Interface](/metadata-documentation/resources/glossary/#archives-portal-admin-interface) to the MMS container or item records, present only for EAD-encoded finding aids</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/archives-ead/">Archives EAD ID</a></dt>
<dd>identifier that correlates EAD-encoded finding aid components to their MMS container or item records, facilitating the display of digitized assets in the Archives Portal</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/barcode/">Barcode</a></dt>
<dd>unique identifier assigned to physical object</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/catnyp/">CATNYP ID (legacy)</a></dt>
<dd>identifier for a bibliographic record in CATNYP, the precursor to the Research Catalog</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/cms-collection/">CMS Collection Identifier</a></dt>
<dd>identifier for the SPEC collection containing an item</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/cms/">CMS Identifier</a></dt>
<dd>unique identifier of an audio or moving image item assigned during inventory in SPEC</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/capture-original-filename/">Capture Original Filename</a></dt>
<dd>filename of the digitized asset</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/digital-gallery-image/">Digital Gallery Image ID</a></dt>
<dd>identifier assigned to an image in Hades, the precursor to the Metadata Management System</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/er/">Electronic Record Package</a></dt>
<dd>number that corresponds to a container of born-digital material described in a finding aid</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/hades-collection-guide/">Hades Collection Guide ID (legacy)</a></dt>
<dd>identifier from legacy Hades Collection Guide page that supported browsing based on collection provenance, bibliographic unit, department, format, and/or topic</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/hades-struc/">Hades struc ID (legacy)</a></dt>
<dd>identifier assigned to a record in Hades, the precursor to the Metadata Management System</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/isan/">International Standard Audiovisual Number</a></dt>
<dd>unique number assigned to audiovisual works and related versions</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/isbn/">International Standard Book Number</a></dt>
<dd>unique number assigned to a particular edition or variation of a published work</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/ismn/">International Standard Music Number</a></dt>
<dd>unique number for the identification of notated music publications</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/iswc/">International Standard Musical Work Code</a></dt>
<dd>unique number assigned to musical works</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/isrc/">International Standard Recording Code</a></dt>
<dd>unique code assigned to sound or music video recording</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/issn/">International Standard Serial Number</a></dt>
<dd>international number standard for serial publications</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/istc/">International Standard Text Code</a></dt>
<dd>unique identifier for text-based works</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/lccn/">Library of Congress Control Number</a></dt>
<dd>unique number associated with a bibliographic record created by the Library of Congress</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/issn-l/">Linking International Standard Serial Number</a></dt>
<dd>international number standard to link serial publications published on several media</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/mss-unit/">MSS Unit ID</a></dt>
<dd>collection-level identifier for an archival collection in the Archives Portal</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/nypl-exhibition/">NYPL Exhibition ID</a></dt>
<dd>identifier for digitized surrogates of material included in exhibitions at the New York Public Library, also known as a TL number (temporary location number)</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/bnumber/">NYPL catalog ID (B-number)</a></dt>
<dd>primary identifier for a bibliographic record in Sierra, where b-number (or "bnumber") is short for bibliographic number</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/other-local/">Other local Identifier</a></dt>
<dd>free-text identifier field that can contain any value, used when adding an identifier that does not align with any predefined Identifier type in the Metadata Management System (MMS)</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/po/">Photo Order</a></dt>
<dd>identifier of the Photo Order (also known as a Public Order) used to track digitization requests submitted to the Library by the public</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/preservica/">Preservica ID</a></dt>
<dd>identifier used by Preservica, the Library's digital preservation software</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/publishers-music-plate-number/">Publisher's music plate number</a></dt>
<dd>plate number assigned to a specific notated music publication by the publisher</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/publisher-assigned-music-number/">Publisher-assigned music number</a></dt>
<dd>number assigned to a musical recording by the publisher other than an issue, matrix, or plate number</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/publisher-assigned-videorecording-number/">Publisher-assigned videorecording number</a></dt>
<dd>number assigned by a publisher to a videorecording</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/oclc/">RLIN/OCLC</a></dt>
<dd>unique identifier assigned by OCLC for a bibliographic record in WorldCat</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/sici/">Serial Item and Contribution Identifier</a></dt>
<dd>code used to uniquely identify specific volumes, articles or other identifiable parts of a serial</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/sound-recording-issue-number/">Sound recording issue number</a></dt>
<dd>number used to identify the issue designation or serial designation assigned by a publisher to a specific musical or nonmusical sound recording, side of a sound recording, or performance on a sound recording</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/sound-recording-matrix-number/">Sound recording matrix number</a></dt>
<dd>alphanumeric code stamped, etched, and/or handwritten, usually between the innermost grooves and the label or hole of a musical or nonmusical sound disc</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/strn/">Standard Technical Report Number</a></dt>
<dd>number assigned to a technical report</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/tms/">TMS ID</a></dt>
<dd>unique numeric identifier assigned to individual objects by the The Museum System (TMS), used by Print Collection and Photography Collection of the Miriam and Ira D. Wallach Division of Art, Prints and Photographs</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/tms-object-number/">TMS Object Number</a></dt>
<dd>local classmark assigned by the Print Collection and Photography Collection of the Miriam and Ira D. Wallach Division of Art, Prints and Photographs in The Museum System (TMS)</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/natgazfid/">U.S. National Gazetteer Feature Name Identifier</a></dt>
<dd>identifier for U.S. National Gazetteer Feature Name</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/uri/">Uniform Resource Identifier</a></dt>
<dd>unique sequence of characters that identifies a logical or physical resource used by web technologies</dd>

<dt><a href="/metadata-documentation/metadata/element/identifier/urn/">Uniform Resource Name</a></dt>
<dd>Uniform Resource Identifier that uses the URN scheme</dd>

</dl>

---

## See Also
- [Top-level Element: &lt;identifier&gt;](https://www.loc.gov/standards/mods/userguide/identifier.html) for official MODS documentation from the Library of Congress
- [Linking Between Systems](/metadata-documentation/workflows/linking/) for an explanation of how identifiers are used to generate links between Library systems
