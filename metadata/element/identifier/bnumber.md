---
layout: page
title: NYPL catalog ID (B-number)
permalink: /metadata/element/identifier/bnumber/
parent: Identifier
grand_parent: By Element
nav_exclude: true
---

# NYPL catalog ID (B-number)
{: .d-inline .v-align-middle .no_toc .mr-2 }
Required if Applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }

Primary identifier for a bibliographic record in [Sierra](/metadata-documentation/resources/glossary/#sierra), where b-number (or "bnumber") is short for bibliographic number
{: .d-block .mt-2 .fs-6 .fw-300 }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Source
- [Sierra](/metadata-documentation/resources/glossary/#sierra) bibliographic records

## Guidelines
- The **NYPL catalog ID (B-number)** identifier is automatically populated into records when [importing MARC records](/metadata-documentation/workflows/create-import/#importing-marc-records)
- If adding a **NYPL catalog ID (B-number)** to a record manually:
    - Include the record type indicator (lower-case `b`) followed by the unique record number (typically 8 digits) as it appears in the address bar when viewing a record in the [Research Catalog](/metadata-documentation/resources/glossary/#research-catalog) or [Legacy Catalog](/metadata-documentation/resources/glossary/#legacy-catalog)
        - If the bnumber is not displaying in the address bar of a record in the [Legacy Catalog](/metadata-documentation/resources/glossary/#legacy-catalog), click **🔗 Permanent link for this record**
    - Do not include the final [check digit](https://documentation.iii.com/sierrahelp/Content/sril/sril_records_numbers.html#check_digit) when retrieving the **NYPL catalog ID (B-number)** from the bibliographic record in Sierra
    - Do not include any spaces or punctuation
- The following guidelines generally apply to usage of **NYPL catalog IDs (B-numbers)** in most cases, but there may be exceptions
    - A **NYPL catalog ID (B-number)** should generally only be assigned to one record in the Metadata Management System
    - A record should generally only have one **NYPL catalog ID (B-number)** assigned at that particular level
    - A record may have multiple **NYPL catalog IDs (B-numbers)** if it is inheriting values from a higher-level collection and/or container
    - If any of the above guidelines do not seem appropriate based on specific record structure or division-specific needs, discuss with the [Manager, Metadata Services](/contact/), before proceeding further

## Format
<dl>
<dt>Preferred structure</dt>
<dd><tt>b<span style="background: #ffccff; border: 1px solid #5c5962;">unique numeric identifier</span></tt></dd>
<dt>Example</dt>
<dd><a href="https://metadata.nypl.org/items/6292814?section=desc_md#:~:text=local_bnumber%3A-,b11689179,-Location"><tt>b<span style="background: #ffccff; border: 1px solid #5c5962;">11689179</span></tt></a></dd>

</dl>

## Inheritance
- Set **NYPL catalog IDs (B-numbers)** added to collections and containers to be **Inheritable**

## See Also
- [Glossary › bnumber](/metadata-documentation/resources/glossary/#bnumber) for a corresponding definition
- [Linking Between Systems › Research Catalog](/metadata-documentation/workflows/linking/#research-catalog) for full explanation of how links between Digital Collections and the library catalog function and are maintained
- [Importing Metadata › Importing MARC Records](/metadata-documentation/workflows/importing/marc/) for the workflow of using a **NYPL catalog IDs (B-numbers)** to import a MARC record into MMS
- [Importing Metadata › Importing MARC Records](/metadata-documentation/workflows/importing/marc/) for the workflow of using a **NYPL catalog ID (B-number)** to import a MARC record into MMS
- [Sierra Reference › How Innovative Systems Store Information › Record Numbers](https://documentation.iii.com/sierrahelp/Content/sril/sril_records_numbers.html) for the vendor's documentation describing record numbers in Sierra