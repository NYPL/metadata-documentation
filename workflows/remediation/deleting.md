---
layout: page
title: Deleting Records & Captures
permalink: /workflows/remediation/deleting/
parent: Remediation
grand_parent: MMS › Workflows
nav_order: 4
nav_exclude: true
---

# Deleting Records & Captures
{: .no_toc }

This page describes the process of deleting records and captures in the Metadata Management System (MMS)

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Overview

{: .warning }
Deleted records and captures cannot be restored within MMS, so take caution to ensure all the guidelines below have been met before proceeding with any deletion.

- Records and captures can only be deleted if they are empty
  - Empty records do not have digital assets associated with the record itself or any child containers or items
  - Empty captures do not have digital assets associated with the capture
- Before deleting a record or capture, ensure it is no longer needed for reference
  - Ensure all necessary metadata elements from an empty record have been replicated elsewhere if needed
  - Ensure the rights profile from an empty record has been replicated elsewhere by a Digitization Coordinator (DC) if needed
    - If a rights profile needs to be moved, follow the [rights](/metadata-documentation/workflows/rights/) workflow and include a link to the empty record

## Deleting Collections

- Review the [deleting records and captures overview](#overview) to ensure your collection is ready to be deleted
- Navigate to the **Overview** tab of the collection record
- At the bottom of the table containing the overview of the collection, click **Delete this collection**
- On the **Delete collection** page:
  - Click **Delete collection** if the collection has no child containers or items
  - Click **Delete collection and all contents** if the collection contains child containers or items that you have verified are no longer needed

## Deleting Containers

- Review the [deleting records and captures overview](#overview) to ensure your container is ready to be deleted
- Navigate to the **Overview** tab of the container record
- At the bottom of the table containing the overview of the container, click **Delete this container**
- On the **Delete container** page:
  - Click **Delete container** if the container has no child containers or items
  - Click **Delete collection and all children** if the container contains child containers or items that you have verified are no longer needed

## Deleting Items

- Review the [deleting records and captures overview](#overview) to ensure your item is ready to be deleted
- Navigate to the **Overview** tab of the item record
- At the bottom of the table containing the overview of the item, click **Delete this item**

## Deleting Captures

{: .note }
See [Troubleshooting Issues](https://nypl.github.io/metadata-documentation/workflows/troubleshooting/) to confirm there is not an issue with the asset before deleting the capture.

- Review the [deleting records and captures overview](#overview) to ensure your capture is ready to be deleted
- Navigate to the **Capture inventory** tab of the item record
- To delete a single capture:
  - In the **Delete** column of the capture’s row, click **X**
- To delete multiple captures:
  - Locate the captures you would like to delete
  - In the **☐** (checkbox) column of the captures' rows, select all the captures you would like to delete
    - Click checkbox at the top of the column to select all captures
  - Open the **Actions on checked captures:** dropdown menu above the captures
  - Select **Delete** and click **Go**
  - Review the pop-up and click **Sounds good, make it so**