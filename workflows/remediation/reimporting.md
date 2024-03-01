---
layout: page
title: Reimporting Metadata
permalink: /workflows/remediation/reimporting/
parent: Remediation
grand_parent: MMS › Workflows
nav_order: 5
nav_exclude: true
---

# Reimporting Metadata
{: .no_toc }

This page describes whether and how to reimport previously-imported records into the Metadata Management System (MMS) from other sources used by the Library to manage description

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Overview
- Metadata [imported](/metadata-documentation/workflows/importing/) into MMS from a [MARC record](/metadata-documentation/workflows/importing/marc/), [finding aid](/metadata-documentation/workflows/importing/finding-aids/), or [TMS record](/metadata-documentation/workflows/importing/tms/) is not automatically kept in sync when changes are made to the source record
- When changes are made to the source record, it may be necessary to reimport metadata to ensure description in MMS aligns with description found in other systems

## Steps (For MSU Staff)

### Determining Whether to Reimport Metadata
1. If you are notified or become aware of updated or new MARC records, finding aids, or TMS records that correspond to records in MMS, cross-reference the MMS record with its source to determine the extent of changes
   1. Manual updates to the record may be preferable if:
      1. You know exactly what the changes in the source record(s) are, and it is not labor-intensive to make the changes in the existing MMS record
      1. There are a large number of captures that would take a significant amount of time to relocate to reimported records
   1. Reimports may be preferable if:
      1. There are significant changes to the descriptive metadata that would be labor-intensive to change manually
      1. The extent of changes is unknown
      1. The structure of the source record differs significantly from the structure of the records in MMS
         1. Any change to the structure of a finding aid typically warrants reimport as [Archives EAD ID](/metadata-documentation/metadata/element/identifier/archives-ead/) and [Archives Components ID](/metadata-documentation/metadata/element/identifier/archives-components/) may have changed
      1. A better, more specific source record is available
         1. New records may be created that describe material at an item-level that was previously described at the collection- or container-level
   1. Programmatic approaches to remediating the existing record may be preferable in particularly complex cases
      1. Discuss with the [Manager, Metadata Services](/metadata-documentation/contact/), to determine next steps
1. For manual updates:
   1. Open the MMS record(s) and make the changes
      1. Ensure new or updated metadata adheres to any relevant [MMS › Metadata](/metadata-documentation/metadata/) guidelines
1. For reimports:
   1. Create a new record following the relevant [import workflow](/metadata-documentation/workflows/importing/):
      1. [MARC Records](/metadata-documentation/workflows/importing/marc/)
      1. [Finding Aids](/metadata-documentation/workflows/importing/finding-aids/)
      1. [TMS Records](/metadata-documentation/workflows/importing/tms/)
   1. [Restructure](/metadata-documentation/workflows/remediation/restructuring/) the new record by [moving records](/metadata-documentation/workflows/remediation/restructuring/#moving-records) from the legacy record(s), [converting record types](/metadata-documentation/workflows/remediation/restructuring/#converting-between-record-types) as needed
      1. If it is unclear where a record or capture belongs, contact the division
      1. [Approve](/metadata-documentation/workflows/approvals/) the new record(s) as you go based on the approval status of the legacy record(s)
   1. If rights are needed for the reimported records, request they be added following the [rights workflow](/metadata-documentation/workflows/rights/)
      1. Include a link to the legacy record(s) if rights were assigned there
   1. Once you have confirmed all metadata elements and rights are in place for the reimported record(s), you may [delete](/metadata-documentation/workflows/remediation/deleting/) the legacy record(s) that are now empty and no longer needed as a result of the reimport
   1. If the legacy record had a [NYPL catalog ID (B-number)](/metadata-documentation/metadata/element/identifier/bnumber/) as an [Identifier](/metadata-documentation/metadata/element/identifier/), ensure that the catalog record’s link to NYPL Digital Collections (DC) gets updated
      1. In the relevant ClickUp task, add a comment indicating the [bnumber](/metadata-documentation/metadata/element/identifier/bnumber/) with the tag `@MSU Sierra Editors`
      1. Do not close the ClickUp task until someone with Sierra edit access has confirmed the catalog record has been updated

### Reviewing a Finding Aid Update from Archival Processing

{: .note }
These steps follow the [related workflow for Archival Processing staff](#notifying-msu-of-an-updated-finding-aid), which will populate a task in [Metadata Services › New Digitization › Metadata Feedback 🔒](https://app.clickup.com/2305128/v/l/26b38-2943).

1. Open the ClickUp task for the finding aid update
1. Check whether an XML file has been attached to the ClickUp task that represents a previous version of the finding aid
   1. If no XML is attached, review details shared by Archival Processing staff to confirm the previous version of the finding aid was not XML-encoded, in which case, skip to the steps to [reimport](#determining-whether-to-reimport-metadata) the finding aid
   1. If an XML file is attached, download it and proceed with the next steps
1. [Download](/metadata-documentation/resources/tips-tricks/#view-xml-in-archives-portal) the current version of the XML from the Archives Portal
1. Compare the two XML files to determine the extent of changes using one of the following tools:
   1. A browser-based tool such as [XML Compare](https://extendsclass.com/xml-diff.html)
   1. A Python library such as [xmldiff](https://pypi.org/project/xmldiff/)
1. Proceed with [determining whether to reimport metadata](#determining-whether-to-reimport-metadata)

## Steps (For Archival Processing Staff)

### Notifying MSU of an Updated Finding Aid
1. Before updating a finding aid in [ArchivesSpace](/metadata-documentation/resources/glossary/#archivesspace), search in the Metadata Management System (MMS) using [Advanced Search 🔒](https://metadata.nypl.org/searches/advanced) to determine whether it has been imported into MMS previously
   1. Select **MSS Unit ID** from the dropdown
   1. Enter the identifier for the archival collection (see [MSS Unit ID › Guidelines](/metadata-documentation/metadata/element/identifier/mss-unit/#guidel))
   1. Click **Search**
1. If the search returns no results, the finding aid can be updated in [ArchivesSpace](/metadata-documentation/resources/glossary/#archivesspace) and the new finding aid XML can be uploaded to the [Archives Portal Admin Interface](/metadata-documentation/resources/glossary/#archives-portal-admin-interface) without the need to notify MSU
1. If the search returns one or more existing record(s), follow the steps based on which form the previous finding aid is in:
   1. PDF finding aid:
      1. Update the finding aid in [ArchivesSpace](/metadata-documentation/resources/glossary/#archivesspace) and upload the new finding aid XML to the [Archives Portal Admin Interface](/metadata-documentation/resources/glossary/#archives-portal-admin-interface)
   1. XML-encoded finding aid:
      1. Download the finding aid XML in its current form from from the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal) before updating
         1. The XML can be downloaded by appending `.xml` to the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal) URL, e.g. <https://archives.nypl.org/mss/3534.xml> 
      1. Update the finding aid in [ArchivesSpace](/metadata-documentation/resources/glossary/#archivesspace) and upload the new finding aid XML to the [Archives Portal Admin Interface](/metadata-documentation/resources/glossary/#archives-portal-admin-interface)
1. Verify that the updated XML is live on the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal) before proceeding
1. Notify MSU of the updated finding aid using its [contact form](/metadata-documentation/contact/form/):
   1. **What would you like to share with us?**: indicate you are submitting a finding aid and whether the XML is new or updated
   1. **Related URL**: URL of updated finding aid in the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal)
   1. **Related division(s)**: division indicated by the **Repository** field of the finding aid
   1. **Your email address**: your NYPL email address
   1. **Attachment(s)**: if applicable, upload the previous version of the finding aid XML that you downloaded prior to updating the finding aid

## See Also
- [Importing Metadata](/metadata-documentation/workflows/importing/) for the different methods of importing metadata into the Metadata Management System (MMS) from other sources used by the Library to manage description
