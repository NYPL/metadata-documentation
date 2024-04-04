---
layout: page
title: Importing TMS Records
permalink: /workflows/importing/tms/
parent: Importing Metadata
grand_parent: MMS › Workflows
nav_order: 4
nav_exclude: true
---

# Importing TMS Records
{: .no_toc }

Describes how to create records in the Metadata Management System (MMS) by importing metadata from records cataloged in [The Museum System](/metadata-documentation/resources/glossary/#the-museum-system) (TMS)

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Overview
- Records for [Print Collection](/metadata-documentation/division/wallach/#print-collection) and [Photography Collection](/metadata-documentation/division/wallach/#photography-collection) cataloged in [The Museum System](/metadata-documentation/resources/glossary/#the-museum-system) (TMS) ~~and accessible via the [Prints & Photographs Online Catalog](https://wallachprintsandphotos.nypl.org/) (PPOC)~~ can be imported into MMS using the [TMS ID](/metadata-documentation/metadata/element/identifier/tms/)
- TMS records always correspond an [item](/metadata-documentation/metadata/record-type/#items) in MMS
  - The **Alternate Titles** field in PPOC may indicate the name of the series to which an item belongs, which may correlate with a collection or container in MMS where the item should be located
  - See [Print Collection](/metadata-documentation/division/wallach/#print-collection) and [Photography Collection](/metadata-documentation/division/wallach/#photography-collection) guidelines to determine what structure is appropriate for an item

{: .warning-title }
> Known Issue
>
> The [Prints & Photographs Online Catalog](https://nypl.github.io/metadata-documentation/resources/glossary/#prints-photographs-online-catalog) was sunset in February 2024. Updated details for locating **TMS ID** values will be added once they are available.
> <small><br>Last checked February 2024</small>

## Steps
1. Determine the appropriate structure for the TMS record, and if necessary, find or create the necessary collection and/or container record(s)
   1. See [Print Collection](/metadata-documentation/division/wallach/#print-collection) and [Photography Collection](/metadata-documentation/division/wallach/#photography-collection) guidelines to determine what structure is appropriate for an item
   1. The **Alternate Titles** field in the [Prints & Photographs Online Catalog](https://wallachprintsandphotos.nypl.org/) may indicate the name of the series to which an item belongs
      1. Search MMS for the value in **Alternate Titles** to check that a record does not already exist that corresponds to the series
      1. Search the [Research Catalog](/metadata-documentation/resources/glossary/#research-catalog) or [Legacy Catalog](/metadata-documentation/resources/glossary/#legacy-catalog) for the value in **Alternate Titles** to see if the series is represented by a MARC record
         1. If you find a MARC record for the series, [import the MARC record](/metadata-documentation/workflows/importing/marc/)
   1. If you have confirmed the item should be in a collection or container and verified that it does not yet exist, [create the collection or container](/metadata-documentation/workflows/creating/) according to the [Print Collection](/metadata-documentation/division/wallach/#print-collection) and [Photography Collection](/metadata-documentation/division/wallach/#photography-collection) guidelines
1. Determine the [TMS ID](/metadata-documentation/metadata/element/identifier/tms/) of the TMS record you want to import
   1. In the [Prints & Photographs Online Catalog](https://wallachprintsandphotos.nypl.org/), the TMS ID can be found as the numeric slug in the URL displayed in your address bar when viewing a record
   1. See [TMS ID](/metadata-documentation/metadata/element/identifier/tms/) for additional context and guidelines
1. Check that a record does not already exist in MMS that corresponds to the TMS record
   1. Search MMS for the [TMS ID](/metadata-documentation/metadata/element/identifier/tms/)
   1. If you receive no results, search MMS for other descriptive metadata displayed in PPOC (such as the **Title** and [**Object Number**](/metadata-documentation/metadata/element/identifier/tms-object-number/)) to confirm a corresponding record does not yet exist as sometimes a TMS ID may be missing
   1. If you find an item record already exists in MMS, use it rather than reimporting the TMS record
1. Navigate to the **Create Item(s) from External IDs** page in MMS:
   1. Via the menu bar using either path:
      1. **Imports** › **Item from External ID**
      1. **Items** › **New** › **Skip form and import from external source**
   1. Alternately, navigate to the record for the collection or container where the item should be located › **Overview** tab › bottom of page › **Import Via** › **External IDs**
      1. Use this method if you found or created a collection or container in the first step
1. Complete the import form
   1. **Collection Owner** (required): select the division displayed in the **Department** field in PPOC
      1. All items imported from TMS records will use either **Wallach Division: Photography Collection** or **Wallach Division: Print Collection**
      1. See [Location](/metadata-documentation/metadata/element/location/)
   1. **Type of Resource** (required): select the appropriate resource type
      1. Generally, items imported from TMS records will use **still image** 
      1. See [Type of Resource](/metadata-documentation/metadata/element/type-of-resource/)
   1. **Specify item(s) parent UUID, if applicable (will override org unit choice)** (optional): the [UUID](/metadata-documentation/resources/glossary/#universally-unique-identifier) of the collection or container where you wish the item to be located
      1. Leave blank if importing a standalone item
      1. Only one location can be specified, so if you are importing multiple TMS records, they must all belong in the same location
      1. This field will be automatically populated if you have navigated to the form via the record for the collection or container where the item should be located
   1. **Type of external IDs** (required): select `tms`
   1. **Enter identifiers, separated by commas (limit 100)** (required): enter the [TMS ID](/metadata-documentation/metadata/element/identifier/tms/)
      1. You may import up to 100 TMS records at a time by separating each bnumber with a comma
   1. Click **Preview**
1. Once you have verified the correct TMS record and metadata appear on the **Would Import As …** page, click **Import these records to MMS**
   1. A confirmation message will be displayed
   1. If importing only one TMS record, the new record will be displayed
   1. If importing more than one TMS record, you can then search MMS for each record to proceed with next steps
1. Review and [restructure](/metadata-documentation/workflows/remediation/restructuring/) your new record(s) as needed
   1. See [Print Collection](/metadata-documentation/division/wallach/#print-collection) and [Photography Collection](/metadata-documentation/division/wallach/#photography-collection) guidelines to determine what structure is appropriate for an item
   1. See [Moving Records](/metadata-documentation/workflows/remediation/restructuring/#moving-records) for how to move content to a new location
1. Proceed with next steps according to the relevant [digitization](/metadata-documentation/workflows/digitization/) or [remediation](/metadata-documentation/workflows/remediation/) workflow