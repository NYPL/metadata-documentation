---
layout: page
title: Exhibitions
permalink: /workflows/digitization/exhibitions/
parent: Digitization
grand_parent: MMS › Workflows
nav_order: 4
nav_exclude: true
---

# Exhibitions
{: .no_toc }

Provides an overview of the workflow for exhibition-related digitization, particularly in relation to metadata creation in the Metadata Management System (MMS)

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Overview

- Library staff may initiate digitization projects that correspond to exhibitions and special displays
- Processes for creating exhibition metadata will vary by library, division, and the exhibition itself
- If the Metadata Services Unit (MSU) should create metadata records for an exhibition in MMS, non-MSU staff can follow the steps in [Requesting Exhibition Metadata Creation](/metadata-documentation/#requesting-exhibition-metadata-creation)
- If non-MSU staff will create metadata records for an exhibition in MMS, they should:
  - Refer to documentation for [Importing Metadata](/metadata-documentation/workflows/importing/) and [Creating New Metadata](/metadata-documentation/workflows/creating/)
  - Add the exhibition identifier to each item in an [Identifier](/metadata-documentation/metadata/element/identifier/po/) element using [NYPL Exhibition ID](/metadata-documentation/metadata/element/identifier/nypl-exhibition/) as the type

## Steps for Non-MSU Staff

### Requesting Exhibition Metadata Creation
{: .d-inline .v-align-middle .mr-2 }
For Non-MSU Staff
{: .d-inline .v-align-middle .label .label-purple .mx-1 }

1. Prepare an exhibition checklist in your preferred spreadsheet platform
   1. Preferred spreadsheet platform (Google Sheets, Airtable, Smartsheet) may be based on your library, division, or the exhibition itself
   1. The [Exhibition Digitization Template - Current](https://docs.google.com/spreadsheets/d/1FcAWekMNHUJ0LuEsTopzOePg6ecDUnVRSO4-PMII36M/edit) can be used as a template
   1. The exhibition checklist _must_ contain the following fields in each row to proceed with metadata creation:
      1. [Exhibition identifier](/metadata-documentation/metadata/element/identifier/nypl-exhibition/), which is typically unique to one item
      1. Source record, e.g.:
         1. Catalog record link containing a [bnumber](/metadata-documentation/metadata/element/identifier/bnumber/)
         1. Finding aid link containing an [MSS Unit ID](/metadata-documentation/metadata/element/identifier/mss-unit/) and which box/folder contains the to-be-digitized item
         1. [TMS ID](/metadata-documentation/metadata/element/identifier/tms/)
      1. If the source record does not provide item-level metadata:
         1. Any additional metadata needed to fulfill [minimum metadata requirements](/metadata-documentation/metadata/element/identifier/nypl-exhibition/)
      1. If the item will only be partially digitized:
         1. Information about which portion of the item should be digitized in the **specify image/s requested** column, e.g. "pages 2-5")
      1. If the spreadsheet contains items that have already been previously digitized:
         1. Clear indication of which items are to be digitized vs. have been previously digitized
         1. For items that have been previously digitized, include at least one of the following:
            1. Link to the item in MMS or Digital Collections
            1. [**UUID**](/metadata-documentation/resources/glossary/#universally-unique-identifier) from MMS
            1. **Image ID** from Digital Collections
   1. Although not required, reference images are helpful if you are able to add them to your spreadsheet
1. Complete the [Contact Form to Notify MSU of Upcoming Digitization](/metadata-documentation/contact/form/upcoming-digitization/)
   1. For **What type of digitization project is it?**, select **Exhibition**
   1. In **Notes for MSU liaison**:
      1. Indicate who will create the metadata (MSU, Digitization Coordinator, division, et al.)
      1. Include source record(s), relevant MMS collections/containers, link to checklist, etc.

## Steps for MSU Staff

### Initiating New Digitization Tracking for Exhibitions
{: .d-inline .v-align-middle .mr-2 }
For MSU Manager
{: .d-inline .v-align-middle .label .label-purple .mx-1 }

1. Review the finalized exhibition checklist to ensure it meets the requirements for digitization listed in [Requesting Exhibition Metadata Creation](/metadata-documentation/#requesting-exhibition-metadata-creation)
1. Update the [Exhibitions Master List 🔒](https://docs.google.com/spreadsheets/d/11-bgNRs2iO6HLG8OQv7quP8KUHCUNxJgC3nIapA0Do0/edit) (or request the MSU liaison do so)
1. Create a new task in [Metadata Services › New Digitization › Digitization Tracking 🔒](https://app.clickup.com/2305128/v/l/6-164664866-1) with the following status and custom fields:
   1. **Status**: **Digitization Idea**
   1. **Project Type**: **Exhibition**
   1. **Digitization By**: **DIS**
   1. **Division(s):** the division(s) that hold the materials in the checklist
   1. **Research Library**: the library(s) that hold the materials in the checklist
   1. Any other custom fields as appropriate
1. Add a link to the exhibition checklist in the description of the task
1. Add an **Assignee** based on [Metadata Liaisons and Contacts 🔒](https://docs.google.com/spreadsheets/d/1P-YDJigon640fTCLP4Ig4-zmzqrX88v5M24ShuxFNVY/edit)
1. Once the exhibition checklist has been finalized
   1. Review the finalized exhibition checklist to ensure it meets the requirements for digitization listed in [Requesting Exhibition Metadata Creation](#requesting-exhibition-metadata-creation)
      1. If any required information is missing, discuss with the [Manager, Metadata Services](/metadata-documentation/contact/)
      1. In special cases, some items may be digitized that have not met the requirements for digitization, but these items should not be [approved](/metadata-documentation/workflows/approvals/) in MMS until the requirements are met
   1. Confirm what item(s) need to be created in MMS
      1. If a [bnumber](/metadata-documentation/metadata/element/identifier/bnumber/), [MSS Unit ID](/metadata-documentation/metadata/element/identifier/mss-unit/), or [TMS ID](/metadata-documentation/metadata/element/identifier/tms/#tms-id) is provided, search it in MMS to verify whether an earlier record for the item(s) or any parent collections or containers already exist(s)
      1. If an initial search using one of the above identifiers yields no results—or if none are provided—search any other relevant metadata, i.e. collection name, title, or creator
      1. For items in collections or containers, navigate through the existing structure to reach the level in the hierarchy where the item would belong
   1. Work with the [Manager, Metadata Services](/metadata-documentation/contact/) to create tasks in [Metadata Services › New Digitization › Metadata Creation 🔒](https://app.clickup.com/2305128/v/l/6-901707354926-1)
      1. Connect individual metadata creation tasks to the exhibition with the **Related Digitization Tracking** relationship

### Creating Exhibition Metadata
{: .d-inline .v-align-middle .mr-2 }
For MSU Staff
{: .d-inline .v-align-middle .label .label-purple .mx-1 }

1. Monitor your [ClickUp notifications 🔒](https://app.clickup.com/2305128/notifications) and [Metadata Services › New Digitization › Metadata Creation 🔒](https://app.clickup.com/2305128/v/l/6-901707354926-1) for exhibition metadata creation tasks that have been assigned to you
   1. Incoming exhibition metadata requests will have the project type **Exhibition** and the status of **To Create Metadata**
1. Refer to documentation for [Importing Metadata](/metadata-documentation/workflows/importing/) and [Creating New Metadata](/metadata-documentation/workflows/creating/)
1. Add the exhibition identifier to each item in an [Identifier](/metadata-documentation/metadata/element/identifier/po/) element using [NYPL Exhibition ID](/metadata-documentation/metadata/element/identifier/nypl-exhibition/) as the type
   1. Add the exhibition identifier at the item level, rather than at the container or collection level, to be clear about what material is tied to the exhibition
   1. In some cases, the exhibition identifier will be for part of an object and [Digital Imaging Services](/metadata-documentation/resources/glossary/#digital-imaging-services) (DIS) will photograph an entire object (e.g., a single page of a pamphlet, a page from a book or periodical)
      1. In these cases, add the exhibition identifier to the record and a [Note](/metadata-documentation/metadata/element/note/) element with the [Type](/metadata-documentation/metadata/element/note/#type) "admin" specifying exactly what part of the item was digitized for the exhibition
1. Item record(s) should remain in Draft status in MMS until the material is digitized
   1. Once an item is digitized, a corresponding task will be generated in [Approvals 🔒](https://app.clickup.com/2305128/v/l/6-180919377-1) and the status can be updated according to the [Approval](/metadata-documentation/workflows/approvals/) workflow
1. Create or update [work order(s)](/metadata-documentation/workflows/digitization/wos/) in MMS
   1. Discuss with contacts for the exhibition—which vary based on division and exhibition—to determine preferences for the work order(s)
   1. If [creating a new work order](/metadata-documentation/workflows/digitization/wos/#creating-a-work-order):
      1. Use the exhibition title as the **Name**
      1. Leave the work order in **Draft** status
      1. [Add records](/metadata-documentation/workflows/digitization/wos/#adding-records-to-a-work-order) you are creating for the exhibition to the work order
1. When metadata creation is complete:
   1. Toggle the ClickUp task Status to **Metadata Created**
   1. Notify exhibition contacts that metadata has been created
   1. It is not necessary to [request rights metadata](/metadata-documentation/workflows/rights/#requesting-rights-metadata) during metadata creation as rights can be requested following digitization during the [approval](/metadata-documentation/workflows/approvals/) process
1. Corresponding [**Approvals 🔒**](https://app.clickup.com/2305128/v/l/6-180919377-1) are connected to the **Digitization Tracking** task as they are received by MSU
1. The **Digitization Tracking** task can be closed once all related digitization and approvals are complete

## See Also
- [NYPL Exhibition ID](/metadata-documentation/metadata/element/identifier/nypl-exhibition/) for guidelines on formatting the identifier assigned to material included in exhibitions at the New York Public Library