---
layout: page
title: Troubleshooting Issues
permalink: /workflows/troubleshooting/
parent: MMS › Workflows
nav_order: 9
---

# Troubleshooting Issues
{: .no_toc }

Describes steps to troubleshoot common technical issues that arise in the Metadata Management System (MMS), Digital Collections (DC), and related systems

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Issues in MMS

### Asset Issues in MMS/DC

#### Image Asset Issues in MMS/DC

For Non-MSU Staff
{: .label .label-purple .m-0 .p-0 }

{: .note }
MSU does not troubleshoot image asset issues, but you can follow the below steps so that the issue can be logged for reference by [Digital Collections Services](/metadata-documentation/resources/glossary/#digital-collections-services).

1. Report issues with image assets via the DC Feedback Form
   1. Open the record in Digital Collections with the image asset issue
   1. Click the **Feedback** button in the lower left corner
   1. Explain the issue and click **Send**

For MSU Staff
{: .label .label-purple .m-0 .p-0 }

1. If you receive a new digitization approval where an image asset has an issue (such as image quality, distortion, or orientation), contact the [Manager, Metadata Services](/metadata-documentation/contact/#our-team)
1. If you encounter issues with image assets outside of the new digitization workflow, submit it via the DC Feedback Form, see steps above

#### Audio and Moving Image Asset Issues in MMS/DC

For Non-MSU Staff
{: .label .label-purple .m-0 .p-0 }

{: .note }
MSU does not troubleshoot audio and moving image asset issues, but you can follow the below steps so that the issue can be logged for future reference.

1. Report playback issues with audio and moving image (AMI) assets via our [contact form](/metadata-documentation/contact/form/)
   1. Your form submission will be routed to the relevant [MSU Liaison 🔒](https://docs.google.com/spreadsheets/d/1P-YDJigon640fTCLP4Ig4-zmzqrX88v5M24ShuxFNVY/edit#gid=0) to be logged

For MSU Staff
{: .label .label-purple .m-0 .p-0 }

1. Add playback issues with audio and moving image (AMI) to the [AMI Asset Issues Log 🔒](https://docs.google.com/spreadsheets/d/1p_12hPb--qOhAuerch07i9ivuzpZEyFABpHhlXpRJ0w/edit) 
1. If the issue was brought to your attention via a [Metadata Feedback](/metadata-documentation/workflows/remediation/feedback/) task in ClickUp, update the task status to **Closed**

### Capture Record Issues in MMS

#### Capture Records in MMS with Broken Image Icons
{: .d-inline .v-align-middle .mr-2 }
For MSU Staff
{: .d-inline .v-align-middle .label .label-purple .mx-1 }

{: .warning-title }
> Known Issue
>
> Orphan image assets are a result of the 2012 migration from [Hades](/metadata-documentation/resources/glossary/#hades) to MMS when the connections between some capture records and their image assets were broken.
> <small><br>Last checked October 2024</small>

1. If you did not create the capture in error, navigate to the **Capture inventory** tab of the capture’s item record
   1. If the item is on a recently created [work order](/metadata-documentation/workflows/digitization/wos/) with a **Draft** __or **Submitted** __status, no action is required as the capture is likely awaiting digitization
   2. If the item is not on a recently created [work order](/metadata-documentation/workflows/digitization/wos/) with a **Draft** or **Submitted** status
      1. If there are **image_id** values present in the **Capture IDs** field, follow the instructions on the [Orphan Image Assets Log](https://docs.google.com/spreadsheets/d/1BB85F6kqpaY9yVmShTf0ksZSH51ZxH4oOPMvXR2tldY/edit?gid=2059872853#gid=2059872853)
      1. If there are no **image_id** values present in the **Capture IDs** field, follow the instructions on the [Captures With No Assets Log](https://docs.google.com/spreadsheets/d/1IUelXEJAtj9qbp0RmVTQ3KxFO7izTt8viQS9j9j-ZAs/edit?gid=2059872853#gid=2059872853)
1. If you created the capture in error, see [Deleting Captures](/metadata-documentation/workflows/remediation/deleting/#deleting-captures)

#### Capture Records in MMS with Inaccurate Captured Status
{: .d-inline .v-align-middle .mr-2 }
For MSU Staff
{: .d-inline .v-align-middle .label .label-purple .mx-1 }

{: .warning-title }
> Known Issue
>
> Occasionally a bug occurs in MMS where marking a work order **Completed** does not trigger **Not captured yet** statuses to be updated to **Captured**. Because capture records with **Not captured yet** status can be deleted in MMS, this may result in accidental deletion of capture records with digitized assets. When capture records with digitized assets are deleted, it results in an orphan image asset, where an image asset exists in the image repository but it is not connected to MMS capture record.
> <small><br>Last checked April 2024</small>

1. Review the capture record for indication that the capture status is inaccurate
   1. From the **Capture inventory** tab of an item:
      1. When the **Thumbnail** displays a thumbnail image or icon _and_ the **Status** column displays **Not captured yet**
   1. From an individual capture record:
      1. When an image or AMI player is displayed _and_ the **Status** row displays **Not captured yet**
1. If you determine capture records meet the criteria above, navigate to any tab of the item record to verify it is not on an active work order
   1. Items on active work orders will display a **On a Work Order, Awaiting Digitization** button
      1. Click **On a Work Order, Awaiting Digitization** to review the work order to confirm it is active
      1. If it appears to be a recent or active work order, no further action is needed
      1. If the work order does not appear to be active but has not yet been marked as **Completed**, report the work to [Manager, Metadata Services](/metadata-documentation/contact/) who will notify Digital Imaging Services (DIS)
   1. Items not on active work orders will not display a **On a Work Order, Awaiting Digitization** button
      1. Report instances that meet all the outlined criteria to [Manager, Metadata Services](/metadata-documentation/contact/) who will notify the [DAM Portfolio](/metadata-documentation/resources/glossary/#dam-portfolio) team

#### Duplicate Captures in MMS
{: .d-inline .v-align-middle .mr-2 }
For MSU Staff
{: .d-inline .v-align-middle .label .label-purple .mx-1 }

See [Suppressing Records › Requesting Duplicate Captures Be Suppressed](/metadata-documentation/workflows/remediation/suppressing/#requesting-duplicate-captures-be-suppressed)

## Issues in Other Systems

### Archives Portal

#### Digitized Content Not Displaying in Archives Portal

See [Linking Between Systems › Archives Portal → Digital Collections](/metadata-documentation/workflows/linking/#archives-portal--digital-collections) for context

For Non-MSU Staff
{: .label .label-purple .m-0 .p-0 }

1. Report issues with digitized content not displaying in the Archives Portal via our [contact form](/metadata-documentation/contact/form/)
   1. Your submission will be routed to the relevant [MSU Liaison 🔒](https://docs.google.com/spreadsheets/d/1P-YDJigon640fTCLP4Ig4-zmzqrX88v5M24ShuxFNVY/edit#gid=0) to be investigated

For MSU Staff
{: .label .label-purple .m-0 .p-0 }

1. Open the ClickUp task generated by a contact form submission
1. Click the **•••** in the upper right corner of the task
   1. Click **Convert to**
   1. Click **Convert to subtask**
   1. Search for and select [Reattaching Archives Portal Images 🔒](https://app.clickup.com/t/86dt148zk)
1. Enhance the subtask
   1. Rename the task to a more descriptive name
   1. Populate the custom fields as appropriate
   1. Describe the extent of the issue in the task description
1. Add a comment with the tag `@MSU Archives Portal Contact(s)`, who will:
   1. Asses whether digitized assets can be manually reattached or other troubleshooting is required
   1. Complete manual reattachment of digitized assets when possible
1. When the digitized assets have been reattached, notify the submitter and update the task status to **Closed**

### Digital Collections

#### Issues with Display and Indexing of Records in Digital Collections

For Non-MSU Staff
{: .label .label-purple .m-0 .p-0 }

{: .note }
MSU does not troubleshoot Digital Collections display and indexing issues, but you can follow the below steps so that the issue can be logged for reference by the [DAM Portfolio](/metadata-documentation/resources/glossary/#dam-portfolio) team.

1. Report issues with the display and indexing of records in Digital Collections via our [contact form](/metadata-documentation/contact/form/)
   1. Your form submission will be routed to the relevant [MSU Liaison 🔒](https://docs.google.com/spreadsheets/d/1P-YDJigon640fTCLP4Ig4-zmzqrX88v5M24ShuxFNVY/edit#gid=0) to be logged

For MSU Staff
{: .label .label-purple .m-0 .p-0 }

1. Add issues with the display and indexing of records in Digital Collections to the [DC Display and Indexing Issues Log 🔒](https://docs.google.com/spreadsheets/d/1a3evibkFk0SIqytac9zUOYmQD2FZVKBk-_Q5Nr5eprE/edit#gid=1283262161)
   1. The issues on this log are periodically reviewed by the [DAM Portfolio](/metadata-documentation/resources/glossary/#dam-portfolio) team
   1. This spreadsheet is also referenced when links to NYPL Digital Collections from the catalog are [refreshed](/metadata-documentation/projects/#links-to-nypl-digital-collections-from-catalog)
1. When the issue has been logged, update the corresponding ClickUp task status to **Closed**

### Research Catalog

#### Broken Links from Research Catalog to Digital Collections

See [Linking Between Systems › Research Catalog → Digital Collections](/metadata-documentation/workflows/linking/#research-catalog--digital-collections) for context

For Non-MSU Staff
{: .label .label-purple .m-0 .p-0 }

1. Report absent or broken links to Digital Collections via our [contact form](/metadata-documentation/contact/form/)
   1. Your submission will be routed to the the relevant [MSU Liaison 🔒](https://docs.google.com/spreadsheets/d/1P-YDJigon640fTCLP4Ig4-zmzqrX88v5M24ShuxFNVY/edit#gid=0) so the Research Catalog record can be updated

For MSU Staff
{: .label .label-purple .m-0 .p-0 }

1. In the relevant ClickUp task generated by a contact form submission, add a comment with the tag `@MSU Sierra Contact(s)`
   1. Include the [bnumber](/metadata-documentation/metadata/element/identifier/bnumber/) and correct [URL](/metadata-documentation/dc/url-structure/) if you are able to determine it
1. When the record has been updated, notify the submitter and update the task status to **Closed**

## See Also
- [Contact Form](/metadata-documentation/contact/form/) for non-MSU staff to report issues to MSU
- [Metadata Feedback](/metadata-documentation/workflows/remediation/feedback/) for an overview of reviewing feedback relating to metadata MMS and DC for MSU staff
- [Removal of Captures with Broken Image Assets [Pilot] 🔒](https://github.com/NYPL/metadata-projects/tree/main/x_completed/2022-2023_removal-of-caps-w-broken-image-assets_pilot) on GitHub for additional documentation of a workflow related to broken image assets