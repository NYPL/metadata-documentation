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

This page describes the process of deleting records in the Metadata Management System (MMS)

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Overview

{: .warning }
Deleted records cannot be restored within MMS, so take caution to ensure all criteria have been met before proceeding with any deletion.

- Records can only be deleted if they are empty
   - See the section that corresponds to the record type for criteria as to what is considered empty
- Before deleting a record, confirm it is no longer needed for reference
   - Ensure all necessary metadata elements from an empty record have been replicated elsewhere if needed
   - Ensure the rights profile from an empty record has been replicated elsewhere by a Digitization Coordinator (DC) if needed
   - If a rights profile needs to be moved, follow the [rights](/metadata-documentation/workflows/rights/) workflow and include a link to the empty record

## Deleting Collections

1. Confirm the collection record is empty, either:
   1. There are no item records within the collection
   1. Item records exist in the collection but do not have associated assets
1. Confirm the collection record is no longer needed for reference, see [deleting records overview](#overview)
1. Navigate to the **Overview** tab of the collection record
1. At the bottom of the table containing the overview of the collection, click **Delete this collection**
1. On the **Delete collection** page:
   1. Click **Delete collection** if the collection has no child containers or items
   1. Click **Delete collection and all contents** if the collection contains child containers or items that you have verified are no longer needed

## Deleting Containers

1. Confirm the container is empty, either:
   1. There are no item records within the container
   1. Item records exist in the container but do not have associated assets
1. Confirm the container record is no longer needed for reference, see [deleting records overview](#overview)
1. Navigate to the **Overview** tab of the container record
1. At the bottom of the table containing the overview of the container, click **Delete this container**
1. On the **Delete container** page:
   1. Click **Delete container** if the container has no child containers or items
   1. Click **Delete collection and all children** if the container contains child containers or items that you have verified are no longer needed

## Deleting Items

1. Confirm the item is empty, either:
   1. There are no capture records attached to the item
   1. Capture records are attached to the item but do not have associated assets
1. Confirm the item record is no longer needed for reference, see [deleting records overview](#overview)
1. Navigate to the **Overview** tab of the item record
1. At the bottom of the table containing the overview of the item, click **Delete this item**

## Deleting Captures

1. Confirm the capture record is empty, both:
   1. There is no value in the **Capture IDs** field on a capture record or on the **Capture inventory** tab of the parent item record
   1. There is not an issue with the asset
      1. See [Troubleshooting Issues](/metadata-documentation/workflows/troubleshooting/)
1. Confirm the container record is no longer needed for reference, see [deleting records overview](#overview)
1. Navigate to the **Capture inventory** tab of the item record
1. To delete a single capture:
   1. In the **Delete** column of the capture’s row, click **X**
1. To delete multiple captures:
   1. Locate the captures you would like to delete
   1. In the **☐** (checkbox) column of the captures’ rows, select all the captures you would like to delete
      1. Click checkbox at the top of the column to select all captures
   1. Open the **Actions on checked captures:** dropdown menu above the captures
   1. Select **Delete** and click **Go**
   1. Review the pop-up and click **Sounds good, make it so**

# See Also
- [MMS Database and SQL Queries 🔒](https://github.com/NYPL/metadata-tools/blob/master/_mms-database-and-sql-queries/README.md) for details on accessing the XML of deleted records