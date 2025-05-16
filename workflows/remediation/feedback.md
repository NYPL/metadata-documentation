---
layout: page
title: Metadata Feedback
permalink: /workflows/remediation/feedback/
parent: Remediation
grand_parent: MMS › Workflows
nav_order: 6
nav_exclude: true
---

# Metadata Feedback
{: .no_toc }

Provides an overview of reviewing feedback relating to metadata in the Metadata Management System (MMS) and Digital Collections (DC) for Metadata Services Unit (MSU) staff

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Overview
- MSU regularly receives feedback on metadata in MMS and DC including corrections and suggestions that are reviewed and implemented as appropriate
- Feedback on metadata may be received by the MSU in several ways including:
  - **DC Feedback Form**: clicking the **Feedback** button in the lower right corner of any page on [NYPL Digital Collections](https://digitalcollections.nypl.org/)
  - **Metadata Reporting Form**: submitted via [Metadata Reporting Form](/metadata-documentation/contact/form/)
  - **Email**: received at metadata [at] nypl [dot] org or by an individual MSU staff member and [forwarded to ClickUp](#forwarding-metadata-feedback-emails-to-clickup)
- Feedback from the **DC Feedback Form** and **Metadata Reporting Form** is routed into the [Metadata Services ClickUp 🔒](https://app.clickup.com/2305128/v/gr/26b38-7748) as it is received

## Steps for MSU Staff

### Forwarding Metadata Feedback Emails to ClickUp
{: .d-inline .v-align-middle .mr-2 }
For MSU Staff
{: .d-inline .v-align-middle .label .label-purple .mx-1 }
1. Retrieve your personalized forwarding email address 
   1. Navigate to [Metadata Services › Remediation Projects › Metadata Feedback 🔒](https://app.clickup.com/2305128/v/gr/26b38-7748) in ClickUp
   1. Click the **•••** next to **Metadata Feedback**
   1. Click **✉ Email to List**
   1. Click **Copy** to copy the email address to your clipboard
   1. [Add the email address to your contacts](https://support.google.com/contacts/answer/1069522?hl=en) with a name you will remember, e.g. `ClickUp list: Metadata Feedback`
1. Forward the email to the `ClickUp list: Metadata Feedback` email address
   1. Optionally, add `<assign me>` in the subject of the email to assign the task to yourself or add `<assign firstnamelastname@nypl.org>` in the subject of the email to assign the task to someone else, replacing `firstnamelastname` with an email address associated with another ClickUp user
1. Open ClickUp and locate the task in your notifications or in [Metadata Services › Remediation Projects › Metadata Feedback 🔒](https://app.clickup.com/2305128/v/gr/26b38-7748)
   1. The new task will use the subject of the email as its task name and the **Feedback Source**: **Email**
   1. Populate custom fields (**Page URL**, **Feedback Tags**, **Division(s)**) and assignee as appropriate
1. Proceed with [reviewing the metadata feedback](#reviewing-metadata-feedback)

### Reviewing Metadata Feedback
{: .d-inline .v-align-middle .mr-2 }
For MSU Staff
{: .d-inline .v-align-middle .label .label-purple .mx-1 }
1. Monitor your [ClickUp notifications 🔒](https://app.clickup.com/2305128/notifications) and [Metadata Services › Remediation Projects › Metadata Feedback 🔒](https://app.clickup.com/2305128/v/gr/26b38-7748) for feedback tasks that have been assigned to you
   1. Each MSU staff member also has a dedicated tab that contains their open feedback tasks grouped by division
      1. To add your respective tab to your favorites in ClickUp, click the **•••** on your tab name and click **⭐ Favorite**
   1. Metadata Feedback views use ClickUp's table display so that the **Feedback Text** and other relevant details are easily seen
1. To open a task, hover over the **Task name** and click the **⤢** button to open the task
1. Once you have selected a feedback task to work on, toggle its status to **In Progress**
1. Review the **Feedback Text** and determine next steps based on the following considerations (discuss with the [Interim Manager, Metadata Services](/metadata-documentation/contact/), if you are uncertain how to proceed):
   1. Has the feedback been submitted by a NYPL staff member or by a patron?
      1. If the feedback was submitted by a NYPL Archival Processing staff member to notify MSU of an updated finding aid, see the related workflow on [Reimporting Metadata](/metadata-documentation/workflows/remediation/reimporting/#reviewing-a-finding-aid-update-from-archival-processing)
   1. Can you verify the accuracy of the feedback, either based on the submitter or through your own research?
   1. Where did the original metadata come from?
   1. Was the metadata transcribed or supplied?
   1. Does the same metadata exist elsewhere in MMS/DC?
   1. Is it appropriate to contact [division staff](https://docs.google.com/spreadsheets/d/1P-YDJigon640fTCLP4Ig4-zmzqrX88v5M24ShuxFNVY/edit) for guidance or confirmation?
   1. Is there any relevant MSU documentation to consult, e.g. [Inclusive & Reparative Description](/metadata-documentation/metadata/inclusive-reparative/)?
1. If you determine that metadata should _not_ be updated:
   1. Add a comment to the ClickUp task, noting that feedback has been reviewed and include your reasoning as to why no action was deemed necessary
   1. Toggle the ClickUp task **Status** to **Closed**
1. If you determine that metadata _should_ be updated:
   1. Update the record(s) in MMS following any relevant guidelines in MSU documentation
   1. If appropriate, a [Note](/metadata/element/note/) element with the [Type](/metadata/element/note/#type) "admin" describing any changes you've made
   1. Determine whether the metadata exists in other systems such as a catalog record or finding aid, and if so, request that it be updated
      1. To request an update to a catalog record, submit a ticket via ServiceNow ([BookOps › Cataloging 🔒](https://nyplprod.service-now.com/nyplsp?id=sc_cat_item&sys_id=37d54594c4504d00f254019b5f40e91f&sysparm_category=2c3832e1139ee740c82e7e276144b022)) with the *Inquiry type*: *Sierra bib record error*
      1. To request an update to a finding aid for a [division served by Archival Processing](https://docs.google.com/document/d/1tiIm0R8P0A_sOH3RUKsPgUKXAThqXT074QeIEokD6uk/edit#heading=h.gh2654hr28xp), complete the [Archival Processing Unit Description Remediation Request](https://docs.google.com/forms/d/e/1FAIpQLSexaz5kCcCdw99U67Z7sVCgemlXpofl9HuegMmGYxcN8zBGCA/viewform) form
      1. To request an update to a finding aid for a division _not_ served by Archival Processing, discuss with the [Interim Manager, Metadata Services](/metadata-documentation/contact/) as the relevant contact can vary by division
   1. If the feedback was submitted by an NYPL staff member and their contact information is included in the task, you may reach out to them to let them know the changes have been made
   1. Add a comment to the ClickUp task, noting that changes were implemented to address the feedback
   1. Ensure the following custom fields are populated in the ClickUp task to support reporting:
      1. **Division(s)**
      1. **Feedback Source**
      1. **Research Library**
      1. **Total Items**
   1. Toggle the ClickUp task **Status** to **Closed**

{: .note-title }
> Note for ClickUp Admin
>
> The steps for routing feedback tasks can be found in [metadata-admin 🔒](https://github.com/NYPL/metadata-admin/blob/main/clickup.md#metadata-feedback).

## See Also
- [Reimporting Metadata › Reviewing a Finding Aid Update from Archival Processing](/metadata-documentation/workflows/remediation/reimporting/#reviewing-a-finding-aid-update-from-archival-processing) for steps that should be followed in the event metadata feedback indicates a finding aid update
- [Inclusive & Reparative Description](/metadata-documentation/metadata/inclusive-reparative/) for guidance on how to create or update metadata according to relevant best practices
- [Search by Image](https://chrome.google.com/webstore/detail/search-by-image/cnojnbdhbhnkbcieeekonklommdnndci) to install a Chrome browser extension that allows you to perform reverse image searches, which may be useful for researching images that are the subject of metadata feedback