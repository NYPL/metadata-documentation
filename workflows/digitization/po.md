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

1. Complete the [Contact Form to Request PO Metadata Creation](/metadata-documentation/contact/form/po/)
1. Once the form is submitted, a new task will be created in [Metadata Services › New Digitization › Metadata Creation 🔒](https://app.clickup.com/2305128/v/l/6-901707354926-1) that:
    1. Is assigned to the submitter of the form, the relevant MSU liaison (based on **Division**), and the Digitization Coordinator (based on **Division**)
    1. Has **Status** of **To Create Metadata**
1. Once metadata is created:
    1. The task's **Status** will appear as **Metadata Created**

## Steps for MSU Staff

### Creating Metadata
{: .d-inline .v-align-middle .mr-2 }
For MSU Staff
{: .d-inline .v-align-middle .label .label-purple .mx-1 }
1. Monitor your [ClickUp notifications 🔒](https://app.clickup.com/2305128/notifications) and [Metadata Services › New Digitization › Metadata Creation 🔒](https://app.clickup.com/2305128/v/l/6-901707354926-1) for metadata creation tasks that have been assigned to you
    1. Incoming PO metadata requests will have a task name that begins with PO and the status of **To Create Metadata**
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
            1. In these cases, add the PO number to the record _and_ a [**Note**](/metadata-documentation/metadata/element/note/) element with the [**Type**](/metadata-documentation/metadata/element/note/#type) "admin" specifying exactly what part of the item was digitized for the PO
    1. Item record(s) should remain in **Draft** status in MMS until the material is digitized
        1. Once an item is digitized, a corresponding task will be generated in [Approvals 🔒](https://app.clickup.com/2305128/v/l/6-180919377-1) and the status can be updated according to the [Approval](/metadata-documentation/workflows/approvals/) workflow
1. Copy the URL(s) of the newly created item(s) in MMS and paste them back into the ClickUp task
    1. If there is only one URL, add it to the **Primary MMS Link** field
    1. If there are multiple URLs, add each to the task description
1. By default, the **Rights** field is set to **Rights Needed** and the **DC (only if Rights Needed)** is populated
    1. If the newly created item(s) already have rights due to inheritance, toggle the rights field to **Rights Completed**
1. When metadata creation is complete:
    1. Add a comment to the ClickUp task with link(s) to the newly created item(s) and include an @ tag of the requesting PRS staff member's name so they receive a notification
    1. Toggle the ClickUp task **Status** to **Metadata Created**

## Post-Metadata Creation
- The next steps following metadata creation include:
    - PRS staff creates the corresponding [Work Order (WO)](/metadata-documentation/workflows/digitization/wos/) and assigns capture identifiers
    - PRS staff coordinate shipment of material to DIS
    - [Copyright and Information Policy](/metadata-documentation/resources/glossary/#copyright-information-policy) staff add rights metadata
    - DIS staff digitizes the requested materials
    - MSU staff [approves](/metadata-documentation/workflows/approvals/) the item(s)
    - Once approved in MMS, item(s) that meet the [criteria for appearance](/metadata-documentation/dc/criteria/) will be accessible on DC
        1. Searching DC using the PO number (without the "PO") will return any publicly accessible items that correspond to that PO
- Pending POs where MSU staff have not yet received the related approval can be found in [Metadata Services › New Digitization › Digitization Tracking › Pending POs 🔒](https://app.clickup.com/2305128/v/l/26b38-9277)
    - Corresponding [Approvals 🔒](https://app.clickup.com/2305128/v/l/6-180919377-1) are connected to the Metadata Creation task as they are received by MSU

## See Also
- [Photo Order](/metadata-documentation/metadata/element/identifier/po/) for more information about the PO identifier
- [Approvals](/metadata-documentation/workflows/approvals/) for an overview of the workflow of approving metadata in MMS
