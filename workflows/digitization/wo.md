---
layout: page
title: Work Orders (WOs)
permalink: /workflows/digitization/wos/
parent: Digitization
grand_parent: MMS › Workflows
nav_order: 3
nav_exclude: true
---

# Work Orders (WOs)
{: .no_toc }

Provides an overview of the workflow for Work Orders (WOs)

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

{: .note }
For best practices and workflows for work orders not covered on this page, contact [Digital Imaging Services (DIS) 🔒](https://lair.nypl.org/-/departments/library-sites-and-services/research-libraries/digital-imaging-services).

## Overview
- A Work Order (WO) is a list in the Metadata Management System (MMS) of capture records ready to be connected with digital assets
   - Work orders typically function as a list of material to be digitized by DIS, but they may also be used for importing assets digitized by external vendors or collaborators
   - Work orders are accessible in MMS at [metadata.nypl.org/work_orders 🔒](https://metadata.nypl.org/work_orders)
   - Work orders are necessary for both internal and vendor digitization
   - Work orders names often correspond to [Public Orders (POs)](/metadata-documentation/workflows/digitization/po/), [Exhibitions](/metadata-documentation/workflows/digitization/exhibitions/), or ongoing digitization projects
   - When the status of a work order is [updated](#updating-the-status-of-a-work-order) to **Completed**, the associated capture records are added to a queue for the system to update their status from **Not Captured Yet** to **Captured**
     - If you notice that a capture record has an asset visible in the **Thumbnail** column of the **Capture inventory** tab of an item but still has the status **Not Captured Yet,** see [Troubleshooting Issues](/metadata-documentation/workflows/troubleshooting/)
- Depending on the relevant digitization workflow, work orders may be created by members of:
   - [Digital Imaging Services (DIS)](/metadata-documentation/resources/glossary/#digital-imaging-services)
   - [Copyright and Information Policy (CIP)](/metadata-documentation/resources/glossary/#copyright-information-policy) ("Digitization Coordinators")
   - [Permissions and Reproduction Services (PRS)](/metadata-documentation/resources/glossary/#permissions-reproduction-services)
   - [Metadata Services Unit (MSU)](/metadata-documentation/resources/glossary/#metadata-services-unit)

## Steps

### Creating a Work Order

{: .note }
New work orders can also be created when [adding records to a work order](#adding-records-to-a-work-order).

1. Navigate to [Work orders 🔒](https://metadata.nypl.org/work_orders)
1. Click **Create new order** at the bottom of the page
1. Enter the metadata for the work order
   1. Only **Name** is required
   1. Consult with DIS on values (if any) for **Priority**, **Photographer**, and **Due date**
   1. All fields are editable after the work order is created, see [Editing a Work Order](#editing-a-work-order)
1. Click **Create**
   1. A confirmation message will be displayed: `Work order created, now you can search items and add them to it.`
1. Proceed with [adding records to the work order](#adding-records-to-a-work-order)

### Editing a Work Order

{: .note }
These steps cover editing a work order's metadata including **Name**, **Due date**, **Photographer**, **Priority**, and **Status**. See corresponding documentation to [add](#adding-records-to-a-work-order) or [remove](#removing-records-from-a-work-order) records from a work order.

1. Locate the work order in MMS and navigate to the **Edit** pop-up
   1. From [Work Orders 🔒](https://metadata.nypl.org/work_orders) or work order search results:
      1. Click **Edit** in the **Actions** column
   1. From a work order:
      1. Click **Edit** under the title of the work order
   1. From a record on an active work order:
      1. Click **On a Work Order, Awaiting Digitization**
      1. Click **Edit** under the title of the work order
   1. From a record on a completed work order:
      1. Click **See Work Order History**
      1. Locate the work order in the list
      1. Click **Edit** in the **Actions** column
1. Edit the work order's metadata fields as needed
1. Click **Save**

### Adding Records to a Work Order
1. Before adding records to a work order, determine which [record type(s)](/metadata-documentation/metadata/record-type/) should be added:
   1. Consult with DIS to determine their preference (if any)
   1. Add the most specific record appropriate
      1. This is typically the lowest record in the hierarchy where everything contained or associated with the record will be digitized, e.g. item > container or container > collection
      1. Do not add a collection or container to a work order unless every item and capture record will be digitized for that work order
      1. Add the collection or container record to a work order only if every item and capture within it will be digitized as this is more efficient than adding every item record
   1. For large collections, create multiple work orders where each contains a subset of the records
      1. Work orders may be slow to load or not load at all if they are too large
1. Confirm the records you wish to add to a work order are not already on other active work orders
   1. An **On a Work Order, Awaiting Digitization** button will display instead of a button to add the record to a work order
   1. Consult with DIS to either:
      1. Ask DIS to [update the **Status**](#updating-the-status-of-a-work-order) of the work order to **Completed**
      1. [Remove](#removing-records-from-a-work-order) the record from the active work order
1. Proceed with next steps based on the record type:
   1. [Collection](#adding-collections-to-a-work-order)
   1. [Container](#adding-containers-to-a-work-order)
   1. [Item](#adding-items-to-a-work-order)
   1. [Capture](#adding-captures-to-a-work-order)

#### Adding Collections to a Work Order

{: .note }
The **Add Collection to Work Order** button may be replaced by an error message on large collections ( `Item too large to add to a work order directly. Please choose a subset of available items or contact admin.`). Instead, create multiple work orders where each contains a subset of the records (see [adding records to a work order](#adding-records-to-a-work-order)).

1. Navigate to any tab of the collection you would like to add to a work order
1. Below the title and UUID of the item record, click **Add Collection to Work Order**
1. If your work order already exists:
   1. Under **Add to an existing order**, use the **search work order name** field to look up the work order by its **Name** or **ID**
      1. Existing work orders can be found at [metadata.nypl.org/work_orders 🔒](https://metadata.nypl.org/work_orders)
   1. If you wish to add only a sub-range of items in the collection, specify the **Start:** and **End:**
   1. Click **Add records to order**
1. If you need to create a new work order:
   1. Under **Or create and add to new order**, use the field to the right of **Or add to new order …** to enter the new work order's **Name**
   1. If you wish to add only a sub-range of items in the collection, specify the **Start:** and **End:**
   1. Click **Create order and add object**
1. Navigate to [**Work orders 🔒**](https://metadata.nypl.org/work_orders) to locate and review your work order

#### Adding Containers to a Work Order
1. Navigate to any tab of the container you would like to add to a work order
1. Below the title and UUID of the item record, click **Add Container to Work Order** 
1. If your work order already exists:
   1. Under **Add to an existing order**, use the **search work order name** field to look up the work order by its **Name** or **ID**
      1. Existing work orders can be found at [metadata.nypl.org/work_orders 🔒](https://metadata.nypl.org/work_orders)
   1. If you wish to add only a sub-range of items in the container, specify the **Start:** and **End:**
   1. Click **Add records to order**
1. If you need to create a new work order:
   1. Under **Or create and add to new order**, use the field to the right of **Or add to new order …** to enter the new work order's **Name**
   1. If you wish to add only a sub-range of items in the container, specify the **Start:** and **End:**
   1. Click **Create order and add object**
1. Navigate to [**Work orders 🔒**](https://metadata.nypl.org/work_orders) to locate and review your work order

#### Adding Items to a Work Order

##### Adding an Single Item to a Work Order
1. Navigate to any tab of the collection you would like to add to a work order
1. Below the title and UUID of the item record, click **Add Item to Work Order** 
1. If your work order already exists:
   1. Under **Add to an existing order**, use the **search work order name** field to look up the work order by its **Name** or **ID**
      1. Existing work orders can be found at [metadata.nypl.org/work_orders 🔒](https://metadata.nypl.org/work_orders)
   1. If you wish to add only a sub-range of captures attached to the item, specify the **Start:** and **End:**
   1. Click **Add records to order**
1. If you need to create a new work order:
   1. Under **Or create and add to new order**, use the field to the right of **Or add to new order …** to enter the new work order's **Name**
   1. If you wish to add only a sub-range of captures attached to the item, specify the **Start:** and **End:**
   1. Click **Create order and add object**
1. Navigate to [**Work orders 🔒**](https://metadata.nypl.org/work_orders) to locate and review your work order

##### Adding Multiple Items to a Work Order
1. Navigate to the **Overview** tab of the collection or container where the item(s) you would like to add to a work order are located
1. In the table that lists items below the overview (and containers, if any), locate the item(s) you would like to add to a work order
1. In the **☐** (checkbox) column of the items' rows, select all the items you would like to add to a work order
   1. Click checkbox at the top of the column to select all the item records visible on the current page
      1. You can adjust the number of items visible on the current page by selecting a different number of items to display next to **Per page:**
      1. To add more items to a work order than can be visible per page, perform this action on multiple pages
1. Open the **Bulk actions on selected items:** dropdown menu above the item records
1. Select **Add to Work Order** and click **Go**
1. In the **The following record(s) will be added to a work order** pop-up:
   1. Verify the capture records listed are accurate
   1. If your work order already exists:
      1. Under **Please select a work order**, use the **search work order name** field to look up the work order by its **Name** or **ID**
         1. Existing work orders can be found at [metadata.nypl.org/work_orders 🔒](https://metadata.nypl.org/work_orders)
      1. Click **Add to order**
   1. If you need to create a new work order:
      1. Under **Or you can create a new work order**, enter the new work order's **Name**
      1. Click **Create order and add object**
1. You will be redirected to the work order where a confirmation message will be displayed: `All records added to workorder.`
   1. If you were not redirected, navigate to [**Work orders 🔒**](https://metadata.nypl.org/work_orders) to locate the work order
   1. Review your work order

#### Adding Captures to a Work Order
1. Navigate to the **Capture inventory tab** of the item where the capture(s) you would like to add is located
1. Locate the capture(s) you would like to add to a work order
1. In the **☐** (checkbox) column of the captures' rows, select the capture(s) you would like to add to the work order
   1. You can adjust the number of captures visible on the current page by selecting a different number of captures to display next to **Per page:**
   1. To add more items to a work order than can be visible per page, perform this action on multiple pages
   1. If you are adding every capture associated with an item to a work order, consider whether it would be more appropriate to [add the item itself to the work order](#adding-an-single-item-to-a-work-order)
1. Open the **Actions on checked captures:** dropdown menu above the captures
1. Select **Add to work order** and click **Go**
1. In the **The following record(s) will be added to a work order** pop-up:
   1. Verify the capture records listed are accurate
   1. If your work order already exists:
      1. Under **Please select a work order**, use the **search work order name** field to look up the work order by its **Name** or **ID**
         1. Existing work orders can be found at [metadata.nypl.org/work_orders 🔒](https://metadata.nypl.org/work_orders)
      1. Click **Add to order**
   1. If you need to create a new work order:
      1. Under **Or you can create a new work order**, enter the new work order's **Name**
      1. Click **Create order and add object**
1. You will be redirected to the work order where a confirmation message will be displayed: `All records added to workorder.`
   1. If you were not redirected, navigate to [**Work orders 🔒**](https://metadata.nypl.org/work_orders) to locate the work order
   1. Review your work order

### Removing Records from a Work Order

{: .note }
Only the exact record that was added to a work order may be removed from a work order. For example, if a collection record was added to a work order, only the collection record may be removed from the work order; container or item records that are part of the collection cannot be removed.

1. From an work order page:
   1. Locate the record in the list
   1. Click **Remove** in the **Actions** column
      1. A confirmation message will be displayed: `Record removed from order.`
1. From a record:
   1. Click **Remove from Current Work Order** below the title and UUID of the record
      1. A confirmation message will be displayed: `Record removed from current work order`

### Deleting a Work Order

{: .note }
Work orders can only be deleted if they are in **Draft** status, see [Updating the Status of a Work Order](#updating-the-status-of-a-work-order).

1. From [Work Orders 🔒](https://metadata.nypl.org/work_orders), work order search results, or **All Associated Orders** for a record:
   1. Click **Destroy** in the **Actions** column
1. From a work order:
   1. Click **Destroy** under the title of the work order

### Updating the Status of a Work Order
{: .d-inline .v-align-middle .mr-2 }
For DIS Staff
{: .d-inline .v-align-middle .label .label-purple .mx-1 }

{: .note }
Work order statuses should only be updated by DIS staff.

1. Navigate to the work order
1. Click **Update** under **Status** in the upper right corner of the work order
1. Select a status from the **Update status:** dropdown menu:
   1. **Draft**
   1. **Submitted**
   1. **Completed**
1. Click **Update**

## See Also

- [How the DIU Uses MMS 🔒](https://docs.google.com/document/d/11Hs9-sPU_3373S_u7oS0P8tMx7GNNV79mgHZmeaNZC4/edit) for related documentation about work orders and MMS created by Digital Imaging Services (DIS)