---
layout: page
title: Deleting Records
permalink: /workflows/remediation/deleting/
parent: Remediation
grand_parent: MMS › Workflows
nav_order: 4
nav_exclude: true
---

# Deleting Records
{: .no_toc }

Describes the process of deleting records in the Metadata Management System (MMS)

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Overview

{: .warning }
Deleted records cannot be restored within MMS, so take caution to ensure all criteria have been met before proceeding with any deletion.

- In general, records should only be deleted in one of the following circumstances:
  - As part of a remediation workflow, e.g. [Restructuring Records](/metadata-documentation/workflows/remediation/restructuring/) or [Reimporting Metadata](/metadata-documentation/workflows/remediation/reimporting/)
  - If records were accidentally created
- Item, container, and collection records can only be deleted if there are no associated captures
  - For items, confirm that the text `No captures yet created for this item.` is present on the **Capture inventory** tab
  - For containers or collections, confirm that the text `Total items in this Container 0` or `Total items in this Collection 0` is present on the **Lightbox view** tab
- Before deleting a record, confirm it is no longer needed for reference
  - Ensure all necessary metadata elements from the record have been replicated elsewhere if needed
  - Ensure the rights profile from the record has been replicated elsewhere by a Digitization Coordinator (DC) if needed
    - If a rights profile needs to be moved, follow the [rights](/metadata-documentation/workflows/rights/) workflow and include a link to the legacy record

## Steps

### Deleting Collections
1. Confirm the collection record meets the [criteria for deletion](/metadata-documentation/workflows/remediation/deleting/#overview)
1. Navigate to the **Overview** tab of the collection record
1. At the bottom of the table containing the overview of the collection, click **Delete this collection**
1. On the **Delete collection** page:
   1. If the collection has no child containers or items, click **Delete collection** 
   1. If the collection contains child containers or items that you have verified are no longer needed, click **Delete collection and all its contents**

### Deleting Containers
1. Confirm the collection record meets the [criteria for deletion](/metadata-documentation/workflows/remediation/deleting/#overview)
1. Navigate to the **Overview** tab of the container record
1. At the bottom of the table containing the overview of the container, click **Delete this container**
1. On the **Delete container** page:
   1. If the container has no child containers or items, click **Delete container**
   1. If the container contains child items that you have verified are no longer needed, click D**elete container and all children** or **Delete container and reassign children**

### Deleting Items
1. Confirm the collection record meets the [criteria for deletion](/metadata-documentation/workflows/remediation/deleting/#overview)
1. Navigate to the **Overview** tab of the item record
1. At the bottom of the table containing the overview of the item, click **Delete this item**

### Deleting Captures
1. Navigate to the **Capture inventory** tab of the item record
1. To delete a single capture:
   1. In the **Delete column** of the capture's row, click **X**
1. To delete multiple captures:
   1. Locate the captures you would like to delete
   1. In the **☐** (checkbox) column of the captures' rows, select all the captures you would like to delete
      1. Click checkbox at the top of the column to select all captures
   1. Open the **Actions on checked captures:** dropdown menu above the captures
   1. Select **Delete** and click **Go**
   1. Review the pop-up and click **Sounds good, make it so**

# See Also
- [MMS Database › Navigation 🔒](https://github.com/NYPL/metadata-tools/blob/master/_mms-database-and-sql-queries/mms-db_navigation.md#descriptive-metadata) for details on accessing the MODS XML of deleted item, container, and collection records
- [Troubleshooting Issues › Capture Record Issues in MMS](/metadata-documentation/workflows/troubleshooting/#capture-record-issues-in-mms) for troubleshooting workflows in cases where capture records appear with no assets or an inaccurate captured status