---
layout: page
title: Importing Finding Aids
permalink: /workflows/importing/finding-aids/
parent: Importing Metadata
grand_parent: MMS › Workflows
nav_order: 3
nav_exclude: true
---

# Importing Finding Aids
{: .no_toc }

Describes how to create records in the Metadata Management System (MMS) by importing metadata from finding aids found in the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal)

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Overview

- Finding aids for [Research Library](/metadata-documentation/resources/glossary/#research-libraries) material accessible via the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal) can be imported into MMS using the [MSS Unit ID](/metadata-documentation/metadata/element/identifier/mss-unit/)
  - Importing EAD-encoded finding aids will replicate the structure of the finding aid within MMS
    - This structure should be preserved as-is except where directed otherwise in the below steps
  - Importing finding aids that are only available as a PDF will create an item record that can then be [converted to a collection](/metadata-documentation/workflows/remediation/restructuring/#converting-items)
- When finding aids in the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal) correspond to a [MARC](/metadata-documentation/resources/glossary/#machine-readable-cataloging) record, it is always preferable to import the finding aid instead of the MARC record

## Steps

1. Determine the [MSS Unit ID](/metadata-documentation/metadata/element/identifier/mss-unit/) of the finding aid you want to import
   1. In the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal), the MSS Unit ID can be found as the numeric slug in the URL displayed in your address bar when viewing a finding aid
   1. See [MSS Unit ID](/metadata-documentation/metadata/element/identifier/mss-unit/) for additional context and guidelines
1. Check that a record does not already exist in MMS that corresponds to the finding aid
   1. Search MMS for the MSS Unit ID
   1. Search MMS for the bnumber of the MARC record that corresponds to the finding aid
      1. The MARC record is linked from the **Call number** field of an [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal) finding aid
      1. The bnumber is found within the URL displayed in your address bar after clicking the link
   1. If you receive no results, search MMS for other descriptive metadata from the finding aid (such as the title) to confirm a corresponding record does not yet exist as sometimes the above identifiers may be missing
   1. If you find a record already exists in MMS and its structure aligns with what you see in the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal), use it rather than reimporting the finding aid
      1. If record exists in MMS, but appears to not align with the current version of the finding aid, [reimporting](/metadata-documentation/workflows/remediation/reimporting/) is recommended
1. Navigate to the **Create Collection from Archives** page in MMS via the menu bar
   1. **Imports** › **Archives Import**
1. Complete the import form
   1. **Enter Archives Collection ID** (required): enter the [MSS Unit ID](/metadata-documentation/metadata/element/identifier/mss-unit/)
   1. Click **Import Finding Aid**
1. You will be redirected to the **Import Status** page
   1. This page can also be accessed via the menu bar
      1. **Imports** › **View all finding aid imports**
   1. Refresh periodically to monitor the **Status** of your import as the page does not auto refresh
   1. Once the import of your finding aid is complete, the **Notes** column will display `Completed.`
   1. Click the number in the **ID** column to view the list of imported components
   1. Click the title of your finding aid that appears after **Details for Import** to view the imported record
1. Review and [restructure](/metadata-documentation/workflows/remediation/restructuring/) your new record(s) as needed
   1. [Convert finding aids that imported as an item](/metadata-documentation/workflows/remediation/restructuring/#converting-items) into a collection if appropriate
      1. Typically, this occurs because the finding aid is not EAD-encoded and is available on the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal) as a PDF
      1. In cases where the full finding aid structure is not imported as it is not EAD-encoded, create containers and items within the collection as appropriate to replicate the structure outlined in the PDF
      1. In cases where the finding aid represents a fully digitized single-item collection (e.g., the [Augustus Porter daybook 🔒](https://metadata.nypl.org/items/6120514)), the record should remain a standalone item
   1. [Convert items](/metadata-documentation/workflows/remediation/restructuring/#converting-items) at the lowest level of the hierarchy in the finding aid that have imported as items into containers as needed
      1. These item records may correspond to boxes and folders, but digitization and description may be done at an item level and therefore the box or folder item record should be converted to a container
      1. If converting an item into a container, set the [Archives EAD ID](/metadata-documentation/metadata/element/identifier/archives-ead/) and the [Note](/metadata-documentation/metadata/element/note/) containing box and folder information to be **Inheritable**
   1. See [By Material › Archival Collections](/metadata-documentation/metadata/material/archival-collections/) for additional guidelines
1. Proceed with next steps according to the relevant [digitization](/metadata-documentation/workflows/digitization/) or [remediation](/metadata-documentation/workflows/remediation/) workflow

## See Also
-  [Archival Collections](/metadata-documentation/metadata/material/archival-collections/) for metadata guidelines specific to archival collections described in MMS