---
layout: page
title: Importing CSV Data
permalink: /workflows/importing/csv/
parent: Importing Metadata
grand_parent: MMS › Workflows
nav_order: 5
nav_exclude: true
---

# Importing CSV Data
{: .no_toc }

This page describes how to create records in the Metadata Management System (MMS) by importing a comma-separated values (CSV) file

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Overview

- Metadata can be created or prepared in a spreadsheet and imported into MMS using CSV import to support bulk metadata creation where source metadata does not exist in a [MARC record](/metadata-documentation/workflows/importing/marc/), [finding aid](/metadata-documentation/workflows/importing/finding-aids/), or [TMS record](/metadata-documentation/workflows/importing/csv/)

## Steps

1. Download the relevant CSV template file:
   1. [Template based on number of captures per item](/metadata-documentation/workflows/importing/csv/mms_template_for_cap_num.csv) (most commonly used template)
   1. [Template based on identifier associated with each capture (one capture per row)](/metadata-documentation/workflows/importing/csv/mms_template_for_cap_ids.csv)
1. Open the CSV template file in your preferred CSV or spreadsheet editor
   1. Prepare your data according to the [CSV data preparation guidelines](#csv-data-preparation-guidelines)
      1. Ensure your data does not contain diacritics as CSV import cannot currently process CSVs contain diacritic characters
   1. Save your new CSV file using UTF encoding
      1. Do not use UTF-8 encoding as doing so can result in a **no method error** during upload
1. Navigate to the **Descriptive metadata import from CSV** page in MMS:
   1. Via the menu bar: **Imports** › **CSV Import**
   1. Alternately, navigate to the record for the collection or container where the item should be located › **Overview** tab › bottom of page › **Import Via** › **CSV**
1. Under **Step 2: Upload file**, select **Choose File** and select your CSV file
1. Under **Step 3: Enter Parent UUID**, enter the [UUID](/metadata-documentation/resources/glossary/#universally-unique-identifier) of the parent collection or container record where your new records should be located
   1. Parent records must already exist within MMS before the CSV import
   1. If you would like to import items within your CSV file to different parent records, leave the text box blank and instead follow the guidelines in [Parent Record](#parent-record) when preparing your CSV data
1. Click **Import**
   1. A banner will display the message `CSV file is processing. You will receive an email notification when completed.`
1. Monitor the email address associated with your MMS account for a message titled `CSV file import completed successfully!`
   1. Once you receive it, click the **View your import** link
1. Review and [restructure](/metadata-documentation/workflows/remediation/restructuring/) your new record(s) as needed
1. Proceed with next steps according to the relevant [digitization](/metadata-documentation/workflows/digitization/) or [remediation](/metadata-documentation/workflows/remediation/) workflow

## CSV Data Preparation Guidelines

{: .note }
The requirements indicated here refer to the technical requirements for your CSV file. For more general guidelines on ensuring the records created by CSV import adhere to local standards, consult [Minimum Metadata Requirements](/metadata-documentation/metadata/guidelines/#minimum-metadata-requirements) and [By Element](/metadata-documentation/metadata/element/).

- <span class="label label-blue fs-1 mb-1 mx-1">Required</span> fields must be present in your CSV file to be imported
- <span class="label label-blue fs-1 mb-1 mx-1">Required if Not Inherited</span> fields must be present in your CSV file if the field is not set to be [inherited](/metadata-documentation/metadata/guidelines/#inheritance) from the parent collection or container record where your new records will be located
  - If you include a field that is already set to be inherited from a parent collection or container, an additional element will be created based on the data from the CSV, and you will need to deduplicate the elements after import
- <span class="label label-blue fs-1 mb-1 mx-1">Required if Not Specified in CSV Import Form</span> fields must be present in your CSV file if the field is _not_ input directly into the CSV import form under **Step 3: Enter Parent UUID**

### Item Number
{: .d-inline .v-align-middle .mr-2 }
Required
{: .d-inline .v-align-middle .label .label-blue .mx-1 }

TK

### Captures
{: .d-inline .v-align-middle .mr-2 }
Required
{: .d-inline .v-align-middle .label .label-blue .mx-1 }

TK

### Identifier
{: .d-inline .v-align-middle .mr-2 }
Required if Not Inherited
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View Full MSU Documentation for Element →]()
{: .d-inline .v-align-middle .text-zeta .ml-2 }

TK

### Title
{: .d-inline .v-align-middle .mr-2 }
Required
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View Full MSU Documentation for Element →]()
{: .d-inline .v-align-middle .text-zeta .ml-2 }

TK

### Location
{: .d-inline .v-align-middle .mr-2 }
Required if Not Inherited
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View Full MSU Documentation for Element →]()
{: .d-inline .v-align-middle .text-zeta .ml-2 }

TK

### Type of Resource
{: .d-inline .v-align-middle .mr-2 }
Required if Not Inherited
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View Full MSU Documentation for Element →]()
{: .d-inline .v-align-middle .text-zeta .ml-2 }

TK

### Date
{: .d-inline .v-align-middle .mr-2 }
Required if Not Inherited
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View Full MSU Documentation for Element →]()
{: .d-inline .v-align-middle .text-zeta .ml-2 }

TK

### Note
{: .d-inline .v-align-middle .mr-2 }
[View Full MSU Documentation for Element →]()
{: .d-inline .v-align-middle .text-zeta .ml-2 }

TK

### Parent Record
{: .d-inline .v-align-middle .mr-2 }
Required if Not Specified in CSV Import Form
{: .d-inline .v-align-middle .label .label-blue .mx-1 }

TK