---
layout: page
title: Suppressing Records
permalink: /workflows/remediation/suppressing/
parent: Remediation
grand_parent: MMS › Workflows
nav_order: 3
nav_exclude: true
---

# Suppressing Records
{: .no_toc }

This page describes the process of suppressing records in the Metadata Management System (MMS)

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Overview

- Suppressing collections, containers, and items should only occur when [addressing harmful content](/metadata-documentation/metadata/inclusive-reparative/#addressing-harmful-content)
  - **Partial content** and **Insufficient metadata** are no longer considered valid reasons for suppressing collections, containers, and items in MMS
    - If available metadata is not sufficient to meet [Minimum Metadata Requirements](/metadata-documentation/metadata/guidelines/), discuss with the [Manager, Metadata Services](/metadata-documentation/contact/#our-team), whether the record should be left in draft status and/or an [admin note](/metadata-documentation/metadata/element/note/#type) should be added to identify uncataloged material
- Suppressing captures should only occur when [suppressing duplicate captures](#suppressing-duplicate-captures-for-msu-staff)
  - See [Troubleshooting Issues](/metadata-documentation/workflows/troubleshooting/) if you encounter other types of problems with capture records or associated assets
- Discuss with the [Manager, Metadata Services](/metadata-documentation/contact/#our-team), before suppressing records for any other reason

## Suppressing Collections

### Suppressing Collections for Harmful Content (For MSU Staff)
1. Review the [suppressing records overview](#overview) to ensure the collection qualifies for suppression
1. Navigate to the **Rights and use** tab of the collection
1. Click the checkbox to **Suppress from website**
1. Do not select a **Reason**
   1. **Partial content** and **Insufficient metadata** are no longer considered valid reasons for suppressing collection records, see [suppressing records overview](#overview)
1. Add an explanation in the **Notes** field of the suppression prompt, e.g. `division requested suppression for harmful content (YYYY-MM-DD INITIALS)`
   1. Replace `YYYY-MM-DD` with the date in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format
   1. Replace `INITIALS` with your initials (see [MMS Database › Quick Reference › User IDs 🔒](https://github.com/NYPL/metadata-tools/blob/master/_mms-database-and-sql-queries/mms-db_quick-reference.md#user-ids))
1. Click **Suppress record**

## Suppressing Containers

### Suppressing Containers for Harmful Content (For MSU Staff)
1. Review the [suppressing records overview](#overview) to ensure the container qualifies for suppression
1. Navigate to the **Rights and use** tab of the container
1. Click the checkbox to **Suppress from website**
1. Do not select a **Reason**
   1. **Partial content** and **Insufficient metadata** are no longer considered valid reasons for suppressing collection records, see [suppressing records overview](#overview)
1. Add an explanation in the **Notes** field of the suppression prompt, e.g. `division requested suppression for harmful content (YYYY-MM-DD INITIALS)`
   1. Replace `YYYY-MM-DD` with the date in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format
   1. Replace `INITIALS` with your initials (see [MMS Database › Quick Reference › User IDs 🔒](https://github.com/NYPL/metadata-tools/blob/master/_mms-database-and-sql-queries/mms-db_quick-reference.md#user-ids))
1. Click **Suppress record**

## Suppressing Items

### Suppressing Items for Harmful Content (For MSU Staff)
1. Review the [suppressing records overview](#overview) to ensure the item qualifies for suppression
1. Navigate to the **Rights and use** tab of the item
1. Click the checkbox to **Suppress from website**
1. Do not select a **Reason**
   1. **Partial content** and **Insufficient metadata** are no longer considered valid reasons for suppressing collection records, see [suppressing records overview](#overview)
1. Add an explanation in the **Notes** field of the suppression prompt, e.g. `division requested suppression for harmful content (YYYY-MM-DD INITIALS)`
   1. Replace `YYYY-MM-DD` with the date in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format
   1. Replace `INITIALS` with your initials (see [MMS Database › Quick Reference › User IDs 🔒](https://github.com/NYPL/metadata-tools/blob/master/_mms-database-and-sql-queries/mms-db_quick-reference.md#user-ids))
1. Click **Suppress record**

## Suppressing Captures

### Suppressing Duplicate Captures (For MSU Staff)
- [Digital Imaging Services (DIS)](/metadata-documentation/resources/glossary/#digital-imaging-services) manages capture suppression
  - Capture suppression only occurs in the event of duplicate captures, see [suppressing records overview](#overview)
  - Follow the steps on [DIS’s](/metadata-documentation/resources/glossary/#digital-imaging-services) [Duplicate captures documentation 🔒](https://docs.google.com/document/d/1o8CiVXBgUkI9kI9duAd0acAKIhEiZj8gnOREEMNUB18/edit)
  - Report duplicate captures to the [Duplicate captures log 🔒](https://docs.google.com/spreadsheets/u/0/d/1jpjta0goQIIaEPesCayWtfSyda5QgGaWxwoiLLyaBmk/edit)

### Suppressing Duplicate Captures (For DIS Staff)
- See [Duplicate captures documentation 🔒](https://docs.google.com/document/d/1o8CiVXBgUkI9kI9duAd0acAKIhEiZj8gnOREEMNUB18/edit)