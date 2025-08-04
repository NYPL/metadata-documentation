---
layout: page
title: Barcode
permalink: /metadata/element/identifier/barcode/
parent: Identifier
grand_parent: By Element
nav_exclude: true
---

# Barcode
{: .d-inline .v-align-middle .no_toc .mr-2 }
Unique identifier assigned to physical object
{: .d-block .mt-2 .fs-6 .fw-300 }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Source
- Assigned by various Library departments during acquisition, cataloging, processing, or collection management workflows and stored in other systems in the Library such as [Sierra](/metadata-documentation/resources/glossary/#sierra) and [SPEC](/metadata-documentation/resources/glossary/#spec)

## Guidelines
- **Barcode**s do not automatically import into MMS when [importing](/metadata-documentation/workflows/importing/) MARC records via finding aid or bnumber but may be added manually
- It may be appropriate to manually add a **Barcode** if:
    - Requested by the division
    - A barcode helps differentiate which specific physical item was digitized, particularly if there are multiple copies and the [**Call number / Shelf Locator**](/metadata-documentation/metadata/element/location/#call-number--shelf-locator) is not unique
    - Specified by corresponding [material](/metadata-documentation/metadata/material/), [division](/metadata-documentation/metadata/division/), or [workflow](/metadata-documentation/workflows/) documentation
- Only add a **Barcode** identifier to the specific record that is 1:1 with the physical material to the barcode has been assigned, e.g.
    - If a barcoded book is digitized in full, assign the **Barcode** identifier at the item-level record for the entire book
    - If a barcoded book is digitized partially, assign the **Barcode** identifier at the collection- or container-level record that represents the entire book, where child item records represent part(s) of the book

## Format

<dl>
<dt>Preferred structure</dt>
<dd><tt><span style="background: #ffccff; border: 1px solid #5c5962;">unique numeric identifier</span></tt></dd>
<dt>Example</dt>
<dd><a href="https://metadata.nypl.org/items/3450522?section=desc_md#:~:text=Barcode%3A-,33333201353840,-Location"><tt><span style="background: #ffccff; border: 1px solid #5c5962;">33333201353840</span></tt></a></dd>
</dl>

## Inheritance
- Do not set **Barcode**s added to collections or containers to be Inheritable

## See Also
- [Audio & Moving Image (AMI) › Identifier](/metadata-documentation/metadata/material/ami/#identifier) for guidelines on the use of identifiers for AMI including Barcode