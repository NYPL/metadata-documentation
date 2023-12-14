---
layout: page
title: Importing MARC Records
permalink: /workflows/importing/marc/
parent: Importing Metadata
grand_parent: MMS › Workflows
nav_order: 2
nav_exclude: true
---

# Importing MARC Records
{: .no_toc }

This page describes how to create records in the Metadata Management System (MMS) by importing metadata from MARC records found in the Library catalog

{: .note }
If a MARC record contains a link to a finding aid, [import the finding aid](/metadata-documentation/workflows/importing/finding-aids) instead of the MARC record.

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Overview

- [MARC](/metadata-documentation/resources/glossary/#machine-readable-cataloging) records for [Research Library](/metadata-documentation/resources/glossary/#research-libraries) material cataloged in [Sierra](/metadata-documentation/resources/glossary/#sierra) can be imported into MMS using the bibliographic number ([bnumber](/metadata-documentation/resources/glossary/#bnumber))
- MARC records can correspond to a [collection](/metadata-documentation/metadata/record-type/#collections), [container](/metadata-documentation/metadata/record-type/#containers), or [item](/metadata-documentation/metadata/record-type/#items) in MMS

## Steps

1. Determine the bnumber of the MARC record you want to import
   1. In the [Research Catalog](/metadata-documentation/resources/glossary/#research-catalog) or [Legacy Catalog](/metadata-documentation/resources/glossary/#legacy-catalog): the bnumber can be found within the URL displayed in your address bar when viewing a record
   1. In [Sierra](/metadata-documentation/resources/glossary/#sierra): the full bnumber is shown at the top of a bibliographic record; remove the final digit (check digit) for the bnumber as it should be used in MMS
   1. See [NYPL catalog ID (B-number)](/metadata-documentation/metadata/element/identifier/bnumber/) for additional context and guidelines
1. Check that a record does not already exist in MMS that corresponds to the bnumber
   1. Search MMS for the bnumber
   1. If you receive no results, search MMS for other descriptive metadata from the MARC record (such as the title) to confirm a corresponding record does not yet exist as sometimes a bnumber may be missing
   1. If you find a record already exists in MMS and it aligns with what you see in the MARC record, use it rather than reimporting the finding aid
      1. If record exists in MMS, but appears to not align with the current version of the MARC record, [reimporting](/metadata-documentation/workflows/remediation/reimporting/) is recommended
1. Determine which [record type](/metadata-documentation/metadata/record-type/) is appropriate for the MARC record and navigate to the corresponding import page in MMS
   1. For [collections](/metadata-documentation/metadata/record-type/#collections): navigate to the **Create Collection(s) from External IDs** page via the menu bar using either path:
      1. **Imports** › **Collection from External ID**
      1. **Collections** › **New** › **Skip form and import from external source**
   1. For [containers](/metadata-documentation/metadata/record-type/#containers): follow the steps above for collections
      1. [Convert the collection to a container](/metadata-documentation/workflows/remediation/restructuring/#converting-collections) after completing the import
   1. For [items](/metadata-documentation/metadata/record-type/#items): navigate to the **Create Item(s) from External IDs** page:
      1. Via the menu bar using either path:
         1. **Imports** › **Item from External ID**
         1. **Items** › **New** › **Skip form and import from external source**
      1. Alternately, navigate to the record for the collection or container where the item should be located › **Overview** tab › bottom of page › **Import Via** › **External IDs**
1. Complete the import form
   1. **Collection Owner** (required): select the appropriate division
      1. See [Location](/metadata-documentation/metadata/element/location/#nypl-divisioncollection)
   1. **Type of Resource** (required): select the appropriate resource type
      1. See [Type of Resource](/metadata-documentation/metadata/element/type-of-resource/)
   1. **Specify item(s) parent UUID, if applicable (will override org unit choice)** (optional, displayed only for items): the [UUID](/metadata-documentation/resources/glossary/#universally-unique-identifier) of the collection or container where you wish the item to be located
      1. Leave blank if importing a standalone item
      1. Only one location can be specified, so if you are importing multiple MARC records, they must all belong in the same location
      1. This field will be automatically populated if you have navigated to the form via the record for the collection or container where the item should be located
   1. **Type of external IDs** (required): select `bnumber`
   1. **Enter identifiers, separated by commas (limit 100)** (required): enter the [bnumber](/metadata-documentation/metadata/element/identifier/bnumber/)
      1. You may import up to 100 MARC records at a time by separating each bnumber with a comma
   1. Click **Preview**
1. Once you have verified the correct MARC record and metadata appear on the **Would Import As …** page, click **Import these records to MMS**
   1. A confirmation message will be displayed
   1. If importing only one MARC record, the new record will be displayed
   1. If importing more than one MARC record, you can then search MMS for each record to proceed with next steps
1. Review and [restructure](/metadata-documentation/workflows/remediation/restructuring/) your new record(s) as needed
   1. See [Converting Between Record Types](/metadata-documentation/workflows/remediation/restructuring/#converting-between-record-types) for how to convert between record types, such as converting a collection to a container
   1. See [Moving Records and Captures](/metadata-documentation/workflows/remediation/restructuring/#moving-records-and-captures) for how to move content to a new location
1. Proceed with next steps according to the relevant [digitization](/metadata-documentation/workflows/digitization/) or [remediation](/metadata-documentation/workflows/remediation/) workflow