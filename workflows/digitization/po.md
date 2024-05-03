---
layout: page
title: Public Orders (POs)
permalink: /workflows/digitization/po/
parent: Digitization
grand_parent: MMS › Workflows
nav_order: 2
nav_exclude: true
---

# Public Orders (POs)
{: .no_toc }

Provides an overview of the workflow for Public Orders (POs), particularly in relation to metadata creation in the Metadata Management System (MMS)

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Overview
- When digitization requests are submitted to the Library by the public, they are tracked internally as POs
    - POs are referred to interchangeably as Public Orders or Photo Orders
- The PO workflow is initiated by [Permissions and Reproduction Services](/metadata-documentation/resources/glossary/#permissions-reproduction-services) (PRS)
- Metadata is created only for material that has not already been digitized
    - Requests for previously digitized materials are delivered to patrons from existing files
- The steps below apply to divisions for which Metadata Services Unit (MSU) staff create metadata records for POs
    - See [Metadata Liaisons and Contacts 🔒](https://docs.google.com/spreadsheets/d/1P-YDJigon640fTCLP4Ig4-zmzqrX88v5M24ShuxFNVY/edit#gid=0&range=F2:F37) to identify who should create metadata records for POs for each division

## Steps for PRS Staff

### Requesting Metadata Creation
{: .d-inline .v-align-middle .mr-2 }
For PRS Staff
{: .d-inline .v-align-middle .label .label-purple .mx-1 }

{: .note }
Before requesting metadata creation, ensure your ClickUp settings are configured to assign you as a watcher to tasks you create in [your notification settings 🔒](https://app.clickup.com/2305128/settings/notifications). Under **Watcher settings: When do you want to be added as a watcher on a task?**, check that **When I create a task or subtask** is selected.

1. Navigate to [Metadata Services › New Digitization › New Digitization Tracking 🔒](https://app.clickup.com/2305128/v/l/6-164664866-1?pr=18903295) in ClickUp
1. From the upper right corner of the list, click **Add Task**
1. Click the **🪄 Templates** button (bottom left of the add task prompt), then click **Use Template**
1. Search for **PO Metadata Creation**, hover over the template, and click **Quick Use**
    1. After using the **PO Metadata Creation** template for the first time, it will appear when clicking the **🪄 Templates** button under **Recent Templates**
1. Replace the task name with the PO number, e.g. `PO1234`
1. Populate template in the task description with any relevant information
    1. Ensure you provide links to **Source Record(s)**, such as a link to the corresponding finding aid or catalog record
    1. If requesting metadata creation for uncataloged material, add a comment on the ClickUp task once it is created and tag the [Manager, Metadata Services](/metadata-documentation/contact/), with an @ symbol
1. Add the **Division** in the custom fields
1. Click **Create Task**, which will create a task that:
    1. Has **Status** of **Create Metadata**
    1. Is assigned to the relevant MSU liaison based on **Division**
    1. Is assigned to Digitization Coordinator for POs to notify them that rights may be needed
    1. Has the person who requested the metadata added to the ClickUp task as a watcher
1. The request will appear in [New Digitization Tracking 🔒](https://app.clickup.com/2305128/v/l/6-164664866-1?pr=18903295) in the **Create Metadata** section

## Steps for MSU Staff

### Creating Metadata
{: .d-inline .v-align-middle .mr-2 }
For MSU Staff
{: .d-inline .v-align-middle .label .label-purple .mx-1 }
1. Monitor your [ClickUp notifications 🔒](https://app.clickup.com/2305128/notifications) and [Metadata Services › New Digitization › New Digitization Tracking 🔒](https://app.clickup.com/2305128/v/l/6-164664866-1) for metadata creation tasks that have been assigned to you
    1. Incoming PO metadata requests will have a task name that begins with PO and the status of **Create Metadata**
1. Review the task description to determine what item(s) need to be created in MMS
    1. If a [bnumber](/metadata-documentation/metadata/element/identifier/bnumber/), [MSS Unit ID](/metadata-documentation/metadata/element/identifier/mss-unit/), or [TMS ID](/metadata-documentation/metadata/element/identifier/tms/#tms-id) is provided, search it in MMS to verify whether an earlier record for the item(s) or any parent collections or containers already exist(s)
    1. If an initial search using one of the above identifiers yields no results—or if none are provided—search any other relevant metadata, e.g. collection name, title, or creator
    1. If an initial search by bnumber yields no results or no bnumber is provided, search any other relevant metadata, e.g. collection name, title, or creator
    1. For items in collections or containers, navigate through the existing structure to reach the level in the hierarchy where the item would belong
1. Create records for the item(s)
    1. Refer to documentation for [Importing Metadata](/metadata-documentation/workflows/importing/) and [Creating New Metadata](/metadata-documentation/workflows/creating/)
    1. Add the PO number to each item in an [**Identifier**](/metadata-documentation/metadata/element/identifier/po/) element using [**Photo Order**](/metadata-documentation/metadata/element/identifier/po/) as the type
        1. Add the PO number _without_ the "PO" at the beginning
        1. Add the PO number at the item level, rather than at the container or collection level, to be clear about what material is tied to the PO
        1. In some cases, the PO will be for part of an object and [Digital Imaging Services](/metadata-documentation/resources/glossary/#digital-imaging-services) (DIS) will photograph an entire object (e.g., a single page of a pamphlet, a page from a book or periodical)
            1. In these cases, add the PO number to the record _and_ a [**Note**](/metadata-documentation/metadata/element/note/) element with the [**Type**](/metadata-documentation/metadata/element/note/#type) "admin" specifying exactly what part of the item was digitized for the the PO
    1. Item record(s) should remain in **Draft** status in MMS until the material is digitized
        1. Once an item is digitized, a corresponding task will be generated in [New Digitization Approvals 🔒](https://app.clickup.com/2305128/v/l/6-180919377-1) and the status can be updated according to the [Approval](/metadata-documentation/workflows/approvals/) workflow
1. Copy the URL(s) of the newly created item(s) in MMS and paste them back into the ClickUp task
    1. If there is only one URL, add it to the **Primary MMS Link** field
    1. If there are multiple URLs, add each to the task description
1. By default, the **Rights** field is set to **Rights Needed** and the **DC (only if Rights Needed)** is populated
    1. If the newly created item(s) already have rights due to inheritance, toggle the rights field to **Rights Completed**
1. When metadata creation is complete:
    1. Add a comment to the ClickUp task, noting that metadata has been created and including an @ tag of the requesting PRS staff member's name so they receive a notification
    1. Toggle the ClickUp task **Status** to **In Progress**

## Post-Metadata Creation
- The next steps following metadata creation include:
    - PRS staff creates the corresponding [Work Order (WO)](/metadata-documentation/workflows/digitization/wos/) and assigns capture identifiers
    - PRS staff coordinate shipment of material to DIS
    - [Copyright and Information Policy](/metadata-documentation/resources/glossary/#copyright-information-policy) (CIP) staff add rights metadata
    - DIS staff digitizes the requested materials
    - MSU staff [approves](/metadata-documentation/workflows/approvals/) the item(s)
    - Once approved in MMS, item(s) that meet the [criteria for appearance](/metadata-documentation/dc/criteria/) will be accessible on DC
        1. Searching DC using the PO number (without the "PO") will return any publicly accessible items that correspond to that PO
- Open POs can be found in [Metadata Services › New Digitization › New Digitization Tracking 🔒](https://app.clickup.com/2305128/v/l/6-164664866-1) with the status **In Progress**
    - Corresponding [New Digitization Approvals 🔒](https://app.clickup.com/2305128/v/l/6-180919377-1) are connected to the New Digitization Tracking task as they are received by MSU
    - The [Manager, Metadata Services](/metadata-documentation/contact/), will close the New Digitization Tracking task once all related approvals are complete

## See Also
- [Photo Order](/metadata-documentation/metadata/element/identifier/po/) for more information about the PO identifier
- [Approvals](/metadata-documentation/workflows/approvals/) for an overview of the workflow of approving metadata in MMS
