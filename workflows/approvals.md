---
layout: page
title: Approvals
permalink: /workflows/approvals/
parent: MMS › Workflows
nav_order: 6
---

# Approvals
{: .no_toc }

Provides an overview of the process of approving records in the Metadata Management System (MMS) to appear on Digital Collections (DC) for Metadata Services Unit (MSU) staff

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Overview
- All records in MMS must be approved by a member of the MSU to meet the [criteria to appear on DC](/metadata-documentation/dc/criteria/)
- The approval workflow is part of new digitization and remediation workflows, often occurring as the last step to make digitized resources available on DC
    - New digitization approvals follow [metadata creation](/metadata-documentation/workflows/create-import/) and [digitization](/metadata-documentation/workflows/digitization/)
    - Backlog approvals are generated through [remediation projects](/metadata-documentation/workflows/remediation/)
    - New digitization approvals should be prioritized over tasks derived from remediation projects

## Steps (For MSU Staff)
1. Monitor your [ClickUp notifications 🔒](https://app.clickup.com/2305128/notifications) and the following lists for approval tasks that have been assigned to you:
    1. [Metadata Services › New Digitization › New Digitization Approvals 🔒](https://app.clickup.com/2305128/v/l/6-180919377-1) for incoming approvals that correspond to newly digitized material
    1. [Metadata Services › Remediation › Remediation Projects › Remediation Tasks 🔒](https://app.clickup.com/2305128/v/l/26b38-8667) for tasks generated as part of remediation projects such as backlog approvals, reimports, et al.
1. Select an approval task to work on and toggle its status to **In Progress**
1. Open the **Work Order Link** (for **New Digitization Approvals**) or **Primary MMS Link** (for **Remediation Projects**) to determine the record(s) in MMS that need to be approved
    1. In MMS:
        1. Determine the scope of the approval by reviewing the item(s) as well as all direct parent records
        1. Note each level of the hierarchy---including any parent collection and containers---that will need to be reviewed and approved separately
        1. Confirm that expected capture(s) are present and appear to be associated with the correct metadata record(s)
    1. In the ClickUp task:
        1. Consult any related tasks (such as **Related Digitization Tracking** or the parent **Remediation Project**) for background
        1. Update the task's title and/or description as needed to aid in your review process
        1. Confirm that the other custom fields (**Division**, **Total Items**, **Research Library**, **Total Captures**, **Project Type**) are completed as applicable
        1. **Rights** and **DC (only if Rights Needed)** custom fields are addressed in a later step
1. Referencing the **Descriptive metadata** tab in MMS for every record within the scope of the approval:
    1. Evaluate the record quality and adjust elements or add enhancements as appropriate and time permits, considering:
        1. Accuracy: does the metadata accurately describe the resource that was digitized?
        1. Completeness: are all [required elements](/metadata-documentation/metadata/guidelines/#minimum-metadata-requirements) populated and formatted correctly
        1. Usefulness: are relevant access points present?
    1. Review the [inherited elements](/metadata-documentation/metadata/guidelines/#inheritance)
        1. Set elements to be inherited or overridden as needed
        1. Try to minimize redundancy where possible
    1. Once you have confirmed all items in the scope of the approval have met the [Minimum Metadata Requirements](/metadata-documentation/metadata/guidelines/#minimum-metadata-requirements), set the status of the item records and any parent records to **Approved**
        1. On the **Overview** tab of an MMS record, look in the **Descriptive metadata** section for the line that begins **Status**
        1. Click the **Edit** link
        1. Toggle **Update status** to **Approved**
        1. Click the **Update** button
1. If additional input is needed before approving any records, toggle the ClickUp task **Status** to **On Hold** and describe what you are waiting for in a comment
    1. If your question is for the division, email the **Primary division contact** listed for that division in the [Metadata Liaisons and Contacts 🔒](https://docs.google.com/spreadsheets/d/1P-YDJigon640fTCLP4Ig4-zmzqrX88v5M24ShuxFNVY/edit)
    1. If your question is for Digital Imaging Services (DIS) staff, tag the [Manager, Metadata Services](/metadata-documentation/contact/), in a comment on the ClickUp task
1. Once all records have been approved, review whether all item records have rights assigned by reviewing the **Rights** section found in the **Overview** tab of the MMS record(s):
    1. If rights information has been specified for all items in the scope of the approval, toggle the **Rights** field of the ClickUp task to **Rights Completed** and proceed with closing the task
        1. **Rights** can either be set at the item-level or inherited from above, both meet the requirement and can be considered completed
    1. If rights information has not been specified for all items in the scope of the approval:
        1. Toggle the **Rights** field of the ClickUp task to **Rights Needed** and the **Status** to **On Hold**
        1. Add the Digitization Coordinator (DC) to the **DC (only if Rights Needed)** field of the ClickUp task
        1. If you are unsure who is the Digitization Coordinator (DC) for a given approval, discuss with the [Manager, Metadata Services](/metadata-documentation/contact/)
        1. Add a comment to the ClickUp task to provide the URLs for the records needing rights and tag the DC with an @ symbol
        1. Once the DC sets the Rights field to Rights Completed, the task status will automatically be updated to **In Progress**
        1. Determine whether the ClickUp task is ready to be closed or should be set back to **On Hold** for any reason, add a comment if necessary
1. When an approval is complete:
    1. Add a comment to the ClickUp task, noting that metadata has been reviewed and approved and that rights are in place
    1. Toggle the ClickUp task **Status** to **Closed**
1. Regularly comb through any approvals with the status of **In Progress** and **On Hold** to confirm their status is accurate and up-to-date

{: .note-title }
> Note for ClickUp Admin
>
> The steps for routing approval tasks can be found in [metadata-admin 🔒](https://github.com/NYPL/metadata-admin/blob/main/clickup.md#new-digitization-approvals)

## See Also

- [Minimum Metadata Requirements](/metadata-documentation/metadata/guidelines/#minimum-metadata-requirements) for a list of the metadata elements required to be approved to appear on Digital Collections
- [Criteria for Appearance](/metadata-documentation/dc/criteria/) for the requirements that must be met in order for the Digital Collections system to display a collection, container, or item