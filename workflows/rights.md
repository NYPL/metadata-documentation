---
layout: page
title: Rights
permalink: /workflows/rights/
parent: MMS › Workflows
nav_order: 7
---

# Rights
{: .no_toc }

Describes the process when Metadata Services Unit (MSU) requests rights metadata be added to records in the Metadata Management System (MMS) by [Copyright and Information Policy](/metadata-documentation/resources/glossary/#copyright-information-policy) (CIP)

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Overview

{: .note }
See [General Guidelines › Rights](/metadata-documentation/metadata/guidelines/#rights) and [Digital Collections › Criteria for Appearance](/metadata-documentation/dc/criteria/) for more information about the role of rights metadata in MMS and how rights codes determine what appears on Digital Collections (DC).

- Rights metadata are added and maintained by [Copyright and Information Policy](/metadata-documentation/resources/glossary/#copyright-information-policy) (CIP)
- Metadata Services Unit (MSU) uses ClickUp to request rights metadata be added to records in the Metadata Management System (MMS)
  - MSU typically requests rights metadata if it has not already been assigned during the [Approval](/metadata-documentation/workflows/approvals/) workflow after digitization is complete and records are approved to ensure captures and records are structured correctly and descriptive metadata are accurate
  - Occasionally, MSU may request rights metadata at other points such as:
    - Prior to digitization as part of a [digitization workflow](/metadata-documentation/workflows/digitization/)
    - Unrelated to new digitization as part of a [remediation workflow](/metadata-documentation/workflows/remediation/)
  - The location of the corresponding ClickUp task will be based on the relevant workflow
    - If you need to create new ClickUp tasks to request rights metadata, discuss with the [Manager, Metadata Services](/metadata-documentation/contact/)
- Staff outside MSU should [contact CIP 🔒](https://lair.nypl.org/-/departments/library-sites-and-services/research-libraries/copyright-information-policy) directly when rights metadata updates or corrections are needed

## Steps for MSU Staff

### Requesting Rights Metadata
{: .d-inline .v-align-middle .mr-2 }
For MSU Staff
{: .d-inline .v-align-middle .label .label-purple .mx-1 }

1. Open the ClickUp task that corresponds to the record that needs rights metadata:
   1. [Metadata Services › New Digitization › New Digitization Approvals 🔒](https://app.clickup.com/2305128/v/l/6-180919377-1) for incoming approvals that correspond to newly digitized material
   1. [Metadata Services › New Digitization › New Digitization Tracking 🔒](https://app.clickup.com/2305128/v/l/6-164664866-1) for tasks that correlate to digitization of materials currently underway
   1. [Metadata Services › Remediation › Remediation Projects › Remediation Tasks 🔒](https://app.clickup.com/2305128/v/l/26b38-8667) for tasks generated as part of remediation projects such as backlog approvals, reimports, etc.
1. Toggle the **Rights** field of the ClickUp task to **Rights Needed**
   1. For approvals, toggle **Status** to **On Hold**
1. Add the Digitization Coordinator (DC) to the **DC (only if Rights Needed)** field of the ClickUp task
   1. The appropriate Digitization Coordinator (DC) is based on the **Project Type** and **Research Library**
   1. If you are unsure who is the Digitization Coordinator (DC), discuss with the [Manager, Metadata Services](/metadata-documentation/contact/)
1. Add a comment to the ClickUp task to specify the URLs for the records needing rights and tag the DC with an @ symbol
1. Once the DC sets the Rights field to **Rights Completed**, a ClickUp bot will add a comment to the task indicating  `✅ rights completed`
   1. For approvals, the task status will automatically be updated to **In Progress**, and the next [approvals steps](/metadata-documentation/workflows/approvals/#steps) can be taken

## Steps for CIP Staff

### Adding Rights Metadata
{: .d-inline .v-align-middle .mr-2 }
For CIP Staff
{: .d-inline .v-align-middle .label .label-purple .mx-1 }

1. When an MSU liaison determines rights metadata are needed, they take the following steps on the corresponding ClickUp tasks:
   1. Set the **Rights** field to **Rights Needed**
   1. Indicate the appropriate Digitization Coordinator (DC) in the **DC (only if Rights Needed)** field
   1. Add a comment specifying the URLs for the records needing rights
1. All ClickUp tasks that indicate rights metadata are needed will appear at [Metadata Services › Rights Needed 🔒](https://app.clickup.com/2305128/v/l/26b38-4647)
   1. It is recommend that DCs "favorite" this page by clicking the name of the **Rights Needed** tab to click **☆ Add to favorites**
   1. By default, favorite views are accessible from the left-side navigation column in ClickUp, but they can be made to appear at all times at the top of the screen by clicking the **📌** icon next to **Favorites** to **Pin Favorites to top**
   1. DCs can also find any tasks assigned to them on the [Home page](https://app.clickup.com/2305128/home), from the[ MSU personalized views](https://app.clickup.com/2305128/v/l/4-18903295-1), and in [notifications](https://app.clickup.com/2305128/notifications)
1. DCs are encouraged to use the comments to discuss any questions for the MSU liaison and provide updates as needed
1. Once rights metadata has been completed, toggle the **Rights** field to **Rights Completed**

## See Also

- [General Guidelines › Rights](/metadata-documentation/metadata/guidelines/#rights) for additional context on the Rights and use tab in MMS, including rights codes
- [Digital Collections › Criteria for Appearance](/metadata-documentation/dc/criteria/) for a list of the factors—including rights metadata—that determine whether records appear on Digital Collections
