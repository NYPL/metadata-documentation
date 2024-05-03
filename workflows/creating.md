---
layout: page
title: Creating New Metadata
permalink: /workflows/creating/
parent: MMS › Workflows
nav_order: 3
---

# Creating New Metadata
{: .no_toc }

Describes if and when it is appropriate to create new metadata in the Metadata Management System (MMS)

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Overview
- In a typical workflow, metadata elements are populated automatically when [importing metadata](/metadata-documentation/workflows/importing/) from other systems:
  - [Importing MARC Records](/metadata-documentation/workflows/importing/marc/)
  - [Importing Finding Aids](/metadata-documentation/workflows/importing/finding-aids/)
  - [Importing TMS Records](/metadata-documentation/workflows/importing/tms/)
- Where source metadata does not exist in a [MARC record](/metadata-documentation/workflows/importing/marc/), [finding aid](/metadata-documentation/workflows/importing/finding-aids/), or [TMS record](/metadata-documentation/workflows/importing/csv/), new metadata can be created in MMS in specific circumstances:
  - Individually, see [steps for creating records](#steps)
  - In bulk, see [Importing CSV data](/metadata-documentation/workflows/importing/csv/)
- The circumstances when it is appropriate to create new metadata records in the Metadata Management System (MMS) are as follows:
  - To describe material at a more granular level than the source record
    - For example, a source record may correspond to a collection or container, and the digitized material warrants item-level description
    - The source record should be imported so that records can be created in the appropriate hierarchy, see [By Record Type](/metadata-documentation/metadata/record-type/)
      - If necessary, a record imported as an item can be [converted into a collection or container](/metadata-documentation/workflows/remediation/restructuring/#converting-items)
    - More granular level description must meet the [Minimum Metadata Requirements](/metadata-documentation/metadata/guidelines/#minimum-metadata-requirements)
  - In cases where an item is digitized partially
    - For example, a source record may correspond to a book that is being partially digitized for a [PO](/metadata-documentation/workflows/digitization/po/) or [exhibition](/metadata-documentation/workflows/digitization/exhibitions/)
    - The source record should be imported so that the structure of the partial digitization is clear
      - If necessary, a record imported as an item can be [converted into a collection or container](/metadata-documentation/workflows/remediation/restructuring/#converting-items)
    - See [By Material](/metadata-documentation/metadata/material/) for material specific-guidelines on structuring partial digitization
  - To group records together in MMS within a synthetic collection
    - For example, material is described in the source record at the container- or item-level, but the division wants the records to be grouped together to represent a thematic or conceptual grouping
    - The collection record can be created manually following any relevant [material](/metadata-documentation/metadata/material/)- or [division](/metadata-documentation/metadata/division/)-specific guidelines, and then source records can be [imported](/metadata-documentation/workflows/importing/) into the collection
- Imported or existing records may also be enhanced with additional descriptive metadata elements
  - This extent of this enhancement is at the metadata creator's discretion based on time and resources available
  - See [By Element](/metadata-documentation/metadata/element/) for local practices for each metadata element and consult any any relevant [material](/metadata-documentation/metadata/material/)- or [division](/metadata-documentation/metadata/division/)-specific guidelines
- Metadata records should _not_ be created in MMS _in lieu_ of material being cataloged in other Library systems such as [Sierra](/metadata-documentation/resources/glossary/#sierra), [ArchivesSpace](/metadata-documentation/resources/glossary/#archivesspace), [TMS](/metadata-documentation/resources/glossary/#the-museum-system), or other [division](/metadata-documentation/metadata/division/)-specific descriptive sources
  - The Metadata Service Unit (MSU) has a policy that all material in MMS is cataloged in other Library systems, even if at a higher level than what has been digitized
  - Discuss with [Manager, Metadata Services](/metadata-documentation/contact/#our-team) before attempting to create a metadata record for uncataloged material
    - In rare cases where uncataloged material is described in MMS with the permission of the Manager, Metadata Services, an [admin note](/metadata-documentation/metadata/element/note/#type) should be added to identify the uncataloged material

## Steps

{: .note }
See [MMS › Metadata › By Record Type](/metadata-documentation/metadata/record-type/) for an overview of the four types of records that contain descriptive content and provide organization for digitized material, each of which have their own properties and descriptive practices.

### Creating Collections
1. Review the [overview](#overview) to confirm it is appropriate to create a new collection record
1. Navigate to the **Create Collection** form in MMS
   1. Via the the menu bar of MMS, navigate to **Collections** › **New**
   1. Via the **Collections** page, click the **Create Collection** button at the top of the page
1. Complete the **Create Collection** form
   1. Add [Title](/metadata-documentation/metadata/element/title/) (required)
   1. Add [Location](/metadata-documentation/metadata/element/location/) (required), typically set to **Inheritable**
   1. Additional [elements](/metadata-documentation/metadata/element/) may be added as appropriate to align the collection record with any relevant [material](/metadata-documentation/metadata/material/)- or [division](/metadata-documentation/metadata/division/)-specific guidelines and ensure all items within it meet the [minimum metadata requirements](/metadata-documentation/metadata/guidelines/#minimum-metadata-requirements)
1. Click **Create Collection**

### Creating Containers

#### Creating Containers in Collections
1. Review the [overview](#overview) to confirm it is appropriate to create a new container record
1. Navigate to the **Overview** tab of the collection where the container should be located in MMS
1. Click **Add Containers** below the overview and above the the item section
1. Complete the **Create Container** form
   1. Add [Title](/metadata-documentation/metadata/element/title/) (required)
   1. Additional [elements](/metadata-documentation/metadata/element/) may be added as appropriate to align the container record with any relevant [material](/metadata-documentation/metadata/material/)- or [division](/metadata-documentation/metadata/division/)-specific guidelines and ensure all items within it meet the [minimum metadata requirements](/metadata-documentation/metadata/guidelines/#minimum-metadata-requirements)
1. Click **Create**

#### Creating Containers in Containers
1. Review the [overview](#overview) to confirm it is appropriate to create a new container record
1. Navigate to the **Overview** tab of the container where the container should be located in MMS
1. Click **Add Sub-Containers** below the overview and above the the item section
1. Complete the **Create Container** form
   1. Add [Title](/metadata-documentation/metadata/element/title/) (required)
   1. Additional [elements](/metadata-documentation/metadata/element/) may be added as appropriate to align the container record with any relevant [material](/metadata-documentation/metadata/material/)- or [division](/metadata-documentation/metadata/division/)-specific guidelines and ensure all items within it meet the [minimum metadata requirements](/metadata-documentation/metadata/guidelines/#minimum-metadata-requirements)
1. Click **Create**

### Creating Items

#### Creating Standalone Items
1. Review the [overview](#overview) to confirm it is appropriate to create a new item record
1. Navigate to the **Create Item** form in MMS
   1. Via the the menu bar of MMS, navigate to **Items** › **New**
   1. Via the **Items** page, click the **Create Item** button at the top of the page
1. Complete the **Create item** form
   1. Add all [minimum metadata requirements](/metadata-documentation/metadata/guidelines/#minimum-metadata-requirements)
   1. Ensure metadata aligns with any relevant [material](/metadata-documentation/metadata/material/)- or [division](/metadata-documentation/metadata/division/)-specific guidelines
   1. Additional [elements](/metadata-documentation/metadata/element/) may be added as appropriate to describe the item
1. Click **Create**

#### Creating Items within Collections or Containers
1. Navigate to the **Overview** tab of the collection or container where the item should be located in MMS
1. Click **Add Items** in the **Items** section
1. In the **Add items** prompt:
   1. Specify the **Number of items to add**
   1. Indicate whether captures should be created for each item in **Create \_\_ captures for each item.**
      1. Captures can also be [created separately](#creating-captures)
      1. If adding captures, specify the **Default capture type** if appropriate
1. Complete the **Create item** form for each item
   1. Add all [minimum metadata requirements](/metadata-documentation/metadata/guidelines/#minimum-metadata-requirements)
   1. Ensure metadata aligns with any relevant [material](/metadata-documentation/metadata/material/)- or [division](/metadata-documentation/metadata/division/)-specific guidelines
   1. Additional [elements](/metadata-documentation/metadata/element/) may be added as appropriate to describe the item
1. If creating a single item:
   1. Click **Create**
1. If creating multiple items, either:
   1. Click **Create and continue to next item**
      1. Toggle **Create next item as duplicate of this one** as appropriate
   1. Click **Create this item and stop**

### Creating Captures

{: .note }
In a typical workflow, captures are not added by MSU staff.

1. Navigate to the **Capture inventory** tab of the item where the capture should be located in MMS
1. Click **Add captures** below the **Capture** heading
1. In the **Add captures** prompt:
   1. Specify the **Number to add:**
   1. Input an optional **Capture name**
   1. Specify the **Type** of capture
1. Click **Create**

## See Also
- [Importing CSV Data](/metadata-documentation/workflows/importing/csv/) for steps for importing a comma-separated values (CSV) file as a method for bulk metadata creation