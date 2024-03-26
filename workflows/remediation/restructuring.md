---
layout: page
title: Restructuring Records
permalink: /workflows/remediation/restructuring/
parent: Remediation
grand_parent: MMS › Workflows
nav_order: 2
nav_exclude: true
---

# Restructuring Records
{: .no_toc }

This page describes different methods of restructuring records in the Metadata Management System (MMS)

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Steps

### Moving Records

#### Moving Collections

- Collection records cannot be moved
  - If you need to move a collection record, it must first be [converted](#converting-collections)

#### Moving Containers

##### Moving Containers Within a Collection

1. Navigate to the **Overview** tab of the collection or container record where the container you would like to move is located
1. In the table that lists containers below the overview, locate the container you would like to move
1. In the **Actions** column of the container's row, click **See actions**
1. In the **Choose Action** pop-up, open the dropdown under **Actions** and select **Move container**
1. In the **Move container** pop-up, begin typing the title or **Record ID** of the container in the **Move to (leave blank for root/collection):** field and select the container from the search results
   1. The **Record ID** of the container can be located as the numeric slug of the URL for the container in MMS, e.g., [https://metadata.nypl.org/containers/**269804**](https://metadata.nypl.org/containers/269804)
   1. To move the item record to the top-level collection where the item is currently located, leave the field blank
   1. Click **Update**
1. On the **Confirm move** page:
   1. Review any **Current inherited elements** compared to the **New inherited elements** to note any metadata elements that will be lost or added as a result of the move that may need to be adjusted in the next step
   1. Once you are ready to complete the move, click **Yes** under **Do you really want to do this?**
1. Review the container in its new location
   1. Ensure no metadata elements were inadvertently lost or added as a result of the move by reviewing the **Descriptive metadata** tab of the container 
   1. Ensure all child items within the container meet the [minimum metadata requirements](/metadata-documentation/metadata/guidelines/#minimum-metadata-requirements) by reviewing the **Descriptive metadata** tab of the respective item record(s)
   1. Ensure all child items within the container have rights assigned by reviewing the **Rights section** found in the **Overview** tab of the respective item record(s)
      1. If rights are needed, follow the [rights](/metadata-documentation/workflows/rights/) workflow and include a link to the previous location of the container if rights were assigned there
1. Once you have confirmed all metadata elements and rights are in place in the container's new location, you may [delete](/metadata-documentation/workflows/remediation/deleting/) any collection or container records that are now empty and no longer needed as a result of moving the container

#### Moving Items

##### Moving Items out of a Collection or Container to Be a Standalone Item

- See [Converting Items](#converting-items)

##### Moving Standalone Items to a Collection or Container

1. Navigate to any tab of the item record
1. Below the title and UUID of the item record, click **Move to new collection**
1. Enter the **Record ID** of the destination collection in the **Enter a collection id** field
   1. The **Record ID** of the collection can be located as the numeric slug of the URL for the collection in MMS, e.g., [https://metadata.nypl.org/collection/**50630**](https://metadata.nypl.org/collection/50630)
   1. Click **Add to Collection**
1. If the destination collection has containers, you will see a page to **Select container**
   1. If you want to move the item to a container, click the radio button for the container where the item should be located and click **Select**
   1. If you want to move the item to the top-level collection, click **Select** without choosing a container
1. On the **Confirm move** page, click **Yes** under **Do you really want to do this?**
   1. Review the **Will be lost** compared to the **Will be gained** to note any metadata elements that will be lost or added as a result of the move that may need to be adjusted in the next step
   1. Once you are ready to complete the move, click **Yes** under **Do you really want to do this?**
1. Review the item in its new location
   1. Ensure no redundant metadata elements were added as a result of the move by reviewing the **Descriptive metadata** tab of the item
   1. Ensure the item retained its rights profile by reviewing the **Rights section** found in the **Overview tab** of the item record

##### Moving Items to a Different Collection

1. Navigate to the **Overview** tab of the collection or container record where the item(s) you would like to move is located
1. In the table that lists items below the overview (and containers, if any), locate the item(s) you would like to move
1. To move a single item:
   1. Locate the item you would like to move
   1. In the **Actions** column of the item's row, open the **Choose action:** dropdown menu and select **Move to new collection**
1. To move multiple items:
   1. Locate the items you would like to move
   1. In the **☐** (checkbox) column of the items' rows, select all the items you would like to move
      1. Click checkbox at the top of the column to select all the items
   1. Open the **Bulk actions on selected items:** dropdown menu above the items
   1. Select **Move to new collection** and click **Go**
1. Enter the **Record ID** of the destination collection in the **Enter a collection id** field
   1. The **Record ID** of the collection can be located as the numeric slug of the URL for the collection in MMS, e.g., [https://metadata.nypl.org/collection/**50630**](https://metadata.nypl.org/collection/50630)
   1. Click **Add to Collection**
1. If the destination collection has containers, you will see a page to **Select container**
   1. If you want to move the item to a container, click the radio button for the container where the item should be located and click **Select**
   1. If you want to move the item to the top-level collection, click **Select** without choosing a container
1. On the **Confirm move** page:
   1. Review **Will be lost** compared to **Will be gained** to confirm [minimum metadata requirements](/metadata-documentation/metadata/guidelines/#minimum-metadata-requirements) will be met once the item is moved to its new location
      1. If necessary, return to the item record to assign required elements and then repeat the above steps
      1. If required elements are not in the item record itself or inherited down in the destination container or collection, you will receive an error message and be unable to move the item
      1. Note any metadata elements that will be lost or added as a result of the move that may need to be adjusted in the next step
   1. Once you are ready to complete the move, click **Yes** under **Do you really want to do this?**
1. Review the item in its new location
   1. Ensure no metadata elements were inadvertently lost or added as a result of the move by reviewing the **Descriptive metadata** tab of the item(s)
   1. Ensure item(s) meet the [minimum metadata requirements](/metadata-documentation/metadata/guidelines/#minimum-metadata-requirements) by reviewing the **Descriptive metadata** tab
   1. Ensure item(s) have rights assigned by reviewing the **Rights section** found in the **Overview** tab
      1. If rights are needed, follow the [rights](/metadata-documentation/workflows/rights/) workflow and include a link to the previous location of the container if rights were assigned there
1. Once you have confirmed all metadata elements and rights are in place in the item's new location, you may [delete](/metadata-documentation/workflows/remediation/deleting/) any collection or container records that are now empty and no longer needed as a result of moving the item

##### Moving Items Within a Collection

1. Navigate to the **Overview** tab of the collection or container record where the item(s) you would like to move is located
1. In the table that lists items below the overview (and containers, if any), locate the item(s) you would like to move
1. To move a single item:
   1. Locate the item record you would like to move
   1. In the **Actions** column of the item's row, open the **Choose action:** dropdown menu and select **Move to new container**
1. To move multiple items:
   1. Locate the item records you would like to move
   1. In the **☐** (checkbox) column of the items' rows, select all the items you would like to move
      1. Click checkbox at the top of the column to select all the item records
   1. Open the **Bulk actions on selected items:** dropdown menu above the item records
   1. Select **Move to new container** and click **Go**
1. In the **Move item to new container** pop-up:
   1. To indicate the destination container by title, begin typing the title in the **Move to (leave blank for root):** field and select the container from the search results
   1. To indicate the destination container by **Record ID**, use the **Or enter valid container id** field
      1. The **Record ID** of the container can be located as the numeric slug of the URL for the container in MMS, e.g., [https://metadata.nypl.org/containers/**269804**](https://metadata.nypl.org/containers/269804)
   1. To move the item record to the top-level collection where the item is currently located, leave both fields blank
   1. Click **Update**
1. On the **Confirm move** page:
   1. Review **Will be lost** compared to **Will be gained** to confirm [minimum metadata requirements](/metadata-documentation/metadata/guidelines/#minimum-metadata-requirements) will be met once the item is moved to its new location
      1. If necessary, return to the item record to assign required elements and then repeat the above steps
      1. If required elements are not in the item record itself or inherited down in the destination container or collection, you will receive an error message and be unable to move the item
   1. Once you are ready to complete the move, click **Yes** under **Do you really want to do this?**
1. Review the item in its new location
   1. Ensure no metadata elements were inadvertently lost or added as a result of the move by reviewing the **Descriptive metadata** tab of the item(s)
   1. Ensure item(s) meet the [minimum metadata requirements](/metadata-documentation/metadata/guidelines/#minimum-metadata-requirements) by reviewing the **Descriptive metadata** tab
   1. Ensure item(s) have rights assigned by reviewing the **Rights section** found in the **Overview** tab
      1. If rights are needed, follow the [rights](/metadata-documentation/workflows/rights/) workflow and include a link to the previous location of the container if rights were assigned there
1. Once you have confirmed all metadata elements and rights are in place in the item's new location, you may [delete](/metadata-documentation/workflows/remediation/deleting/) any collection or container records that are now empty and no longer needed as a result of moving the item

#### Moving Captures

1. Navigate to the **Capture inventory** tab of the item where the capture(s) you would like to move is located
1. Locate the capture(s) you would like to move
1. To move a single capture:
   1. In the **Move** column of the capture's row, click **Move to new item**
1. To move multiple captures:
   1. Locate the captures you would like to move
   1. In the **☐** (checkbox) column of the captures' rows, select all the captures you would like to move
      1. Click checkbox at the top of the column to select all captures
   1. Open the **Actions on checked captures:** dropdown menu above the captures
   1. Select **Move to new item** and click **Go**
1. In the pop-up:
   1. To indicate the destination item by title, begin typing the title in the **Parent item:** field and select the item from the search results
   1. To indicate the destination item by **Record ID**, use the **Or enter valid item id** field
      1. The **Record ID** of the item can be located as the numeric slug of the URL for the item in MMS, e.g., [https://metadata.nypl.org/items/**4902530**](https://metadata.nypl.org/items/4902530)
   1. Click **Move**
1. Review the capture in its new location
   1. Use the **Reorder** or **Reorder (with thumbnails)** if you need to change the order of the capture(s)
1. Once you have confirmed the capture has been successfully to its new location, you may [delete](/metadata-documentation/workflows/remediation/deleting/) any item records that are now empty and no longer needed as a result of moving the capture

### Converting Between Record Types

#### Converting Collections

- Collection records can only be converted if there are no records within the collection
- Collection records can only be converted to item records

##### Converting Collections to Items

1. Navigate to any tab of the collection record
1. Below the title and UUID of the item record, click **Change object type**
1. Confirm **Item** is selected in the dropdown menu and click **Submit**
1. The item can remain a standalone item or be [moved to a collection or container](#moving-standalone-items-to-a-collection-or-container)

#### Converting Containers

- Container records can only be converted if there are no records within the container
- Container records can only be converted to item records

##### Converting Containers to Items

1. Navigate to any tab of the container record
1. Below the title and UUID of the item record, click **Change object type**
1. Confirm **Item** is selected in the dropdown menu and click **Submit**

#### Converting Items

- Item records can only be converted if there are no capture records attached to the item record
- The workflow for converting item records is based on an item's current location and destination

##### Converting Standalone Items to Collections

1. Navigate to any tab of the item record
1. Below the title and UUID of the item record, click **Change object type**
1. Confirm **Collection** is selected in the dropdown menu and click **Submit**

##### Converting Items Within a Collection to Containers

1. Navigate to any tab of the item record
1. Below the title and UUID of the item record, click **Change object type**
1. Confirm **Container** is selected in the dropdown menu and click **Submit**

##### Converting Items Within a Collection or Container to Standalone Items

1. Navigate to the **Overview** tab of the collection or container record where the item you would like to convert is located
1. In the table that lists items below the overview (and containers, if any), locate the item you would like to convert
1. In the **Actions** column of the item's row, open the **Choose action:** dropdown menu and select **Convert to standalone**
1. Review the item in its new location
   1. Ensure no metadata elements were inadvertently lost as a result of the move by reviewing the **Descriptive metadata** tab of the item
   1. Ensure item meets the [minimum metadata requirements](/metadata-documentation/metadata/guidelines/#minimum-metadata-requirements) by reviewing the **Descriptive metadata** tab
   1. Ensure item(s) have rights assigned by reviewing the **Rights section** found in the **Overview** tab
      1. If rights are needed, follow the [rights](/metadata-documentation/workflows/rights/) workflow and include a link to the previous location of the container if rights were assigned there

#### Converting Captures

- Capture records cannot be converted

## See Also

- [Record Types](/metadata-documentation/metadata/record-type/) for an overview of the four types of records in MMS that contain descriptive content and provide organization for digitized material
