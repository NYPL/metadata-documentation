---
layout: page
title: Photo Order
permalink: /metadata/element/identifier/po/
parent: Identifier
grand_parent: By Element
nav_exclude: true
---

# Photo Order
{: .d-inline .v-align-middle .no_toc .mr-2 }
Required if Applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
Repeatable
{: .d-inline .v-align-middle .label .label-green .mx-1 }

Identifier of the Photo Order (also known as a [Public Order](/metadata-documentation/resources/glossary/#public-order)) used to track digitization requests submitted to the Library by the public
{: .d-block .mt-2 .fs-6 .fw-300 }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Source
- [Permissions and Reproduction Services](/metadata-documentation/resources/glossary/#permissions-reproduction-services) (PRS) team

## Guidelines
- Digitization requests submitted to the Library by the public are tracked internally using a sequential PO number recognizable as they begin with "PO," e.g. "PO64824," which can be found in the following places:
  - [New Digitization › New Digitization Approvals 🔒](https://app.clickup.com/2305128/v/l/6-180919377-1) in ClickUp
  - [New Digitization › Digitization Tracking 🔒](https://app.clickup.com/2305128/v/l/6-164664866-1) in ClickUp
  - [Work Orders 🔒](https://metadata.nypl.org/work_orders) in the Metadata Management System (MMS)
- When adding a **Photo Order** value to a record in MMS, only include numeric characters as the identifier value, e.g., "64824" rather than "PO64824"
- Add **Photo Order** values at the item-level
  - A **Photo Order** value may be added to multiple items
  - If an item has more than one **Photo Order** value, add an admin note to indicate which captures are associated with which **Photo Order**
  - If a **Photo Order** value only applies to some of an item's captures rather than all of the captures, add an admin note to indicate which captures are associated with the **Photo Order**

## Format

<dl>
<dt>Preferred structure</dt>
<dd><tt><span style="background: #ffccff; border: 1px solid #5c5962;">unique numeric identifier</span></tt></dd>
<dt>Example</dt>
<dd><a href="https://metadata.nypl.org/items/6269140?section=desc_md#:~:text=Photo%20Order%3A-,64824,-Location"><tt><span style="background: #ffccff; border: 1px solid #5c5962;">64824</span></tt></a></dd>
</dl>

## Inheritance
- Not applicable as **Photo Order** should be assigned at the item level

## See Also
- [Public Orders (POs)](/metadata-documentation/workflows/digitization/po/) for a step-by-step of workflow for digitizing materials for Public Orders
- [Digitization Tracking 🔒](https://app.clickup.com/2305128/v/l/6-164664866-1) for ClickUp tasks that correlate to Public Orders
