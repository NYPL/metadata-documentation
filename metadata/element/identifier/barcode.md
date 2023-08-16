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
- Unless specified by corresponding [material](/metadata-documentation/metadata/material/), [division](/metadata-documentation/metadata/division/), or [workflow](/metadata-documentation/workflows/) documentation, it is not necessary to add a **Barcode** to records
    - **Barcode**s do not import into MMS when [importing](/metadata-documentation/workflows/import/) MARC records via finding aid, bnumber, or TMS import
    - **Barcode**s correspond to a specific physical item, so particular care is required when adding barcodes to records in MMS to ensure accuracy to the particular copy or version that was digitized

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
- [Audio and Moving Image (AMI) › Identifier](/metadata-documentation/metadata/material/ami/#identifier) for guidelines on the use of identifiers for AMI including Barcode