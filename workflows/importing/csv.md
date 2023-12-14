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

- Populate an **item_number** column with a unique, sequential number for each item
  - Enter `1` for the first row
  - Add additional rows containing sequential numbers (`1`, `2`, `3`, `4`…) to correspond to the number of items you wish to create

### Captures
{: .d-inline .v-align-middle .mr-2 }
Required
{: .d-inline .v-align-middle .label .label-blue .mx-1 }

- Populate a captures column with the header that corresponds to the method appropriate for your needs:
  - By number of captures per item:
    - Start with the [template based on number of captures per item](/metadata-documentation/workflows/importing/csv/mms_template_for_cap_num.csv)
    - Populate the **cap_num** column with the number of captures for each item in the corresponding row
      - The **cap_num** value can be zero if you do not wish to add any captures to the item
    - The **item_number** column should increase by an increment of one for each row (i.e., `1`, `2`, `3`, `4`…) as each row represents a single item
  - By identifier associated with each capture:
    - Start with the [template based on identifier associated with each capture (one capture per row)](/metadata-documentation/workflows/importing/csv/mms_template_for_cap_ids.csv)
    - Populate a **cap_iden** column to add each capture identifier to its own row
      - Enter capture identifiers in sequence
    - Adjust the **item_number** column to indicate how captures are grouped together by repeating numbers for captures that correspond to a single item
      - For example, three items with two captures each can be configured with six rows, with the item numbers `1`, `1`, `2`, `2`, `3`, `3`
      - Enter values for additional fields in the first row that corresponds to a particular item number as the data does not need to be repeated for each capture

### Identifier
{: .d-inline .v-align-middle .mr-2 }
Required if Not Inherited
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View Full MSU Documentation for Element →](/metadata-documentation/metadata/element/identifier/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- Populate an identifier column with the header that corresponds to the [type of identifier](/metadata-documentation/metadata/element/identifier/#type) you wish to add for each item

### Title
{: .d-inline .v-align-middle .mr-2 }
Required
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View Full MSU Documentation for Element →](/metadata-documentation/metadata/element/title/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- Populate a **titleInfo_title** column with the [title](/metadata-documentation/metadata/element/title/#title-1) for each item
  - Add additional columns as needed to provide additional title fields, such as [subtitle](/metadata-documentation/metadata/element/title/#subtitle) **(titleInfo_subTitle**), [part number](/metadata-documentation/metadata/element/title/#part-number) (**titleInfo_partNumber**), and [part name](/metadata-documentation/metadata/element/title/#part-name) (**titleInfo_partName**)

### Location
{: .d-inline .v-align-middle .mr-2 }
Required if Not Inherited
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View Full MSU Documentation for Element →](/metadata-documentation/metadata/element/location/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- Populate a **location_division** column with the [Library division](/metadata-documentation/metadata/element/location/#nypl-divisioncollection) that owns each item
  - Use the division's three-letter code from the [Organizational Unit code list](http://metadata.nypl.org/org_units/list), e.g. `THE` for the `Billy Rose Theatre Division`
  - If the [Location](/metadata-documentation/metadata/element/location/) element is set to be inherited from a parent record, you do not need to include a **location_division** column in the CSV file
  - If no **location_division** is provided and the item does not inherit its [Location](/metadata-documentation/metadata/element/location/) from a parent record, the item will be imported with the location `UNK`
- Populate a **location_shelfLocator** column with the [call number or shelf locator](/metadata-documentation/metadata/element/location/#call-number--shelf-locator) information for the item
  - **location_division** is required in order to use **location_shelfLocator**

### Type of Resource
{: .d-inline .v-align-middle .mr-2 }
Required if Not Inherited
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View Full MSU Documentation for Element →](/metadata-documentation/metadata/element/type-of-resource/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- Populate a **typeOfResource_value** column with the type of resource for each item
  - Add additional columns as needed to indicate attributes, such as whether the type of resource should be marked as [primary](/metadata-documentation/metadata/element/type-of-resource/#primary) (**typeOfResource_usage**), a [manuscript](/metadata-documentation/metadata/element/type-of-resource/#manuscript) (**typeOfResource_manuscript**), or a [collection](/metadata-documentation/metadata/element/type-of-resource/#collection) (**typeOfResource_collection**)

### Date
{: .d-inline .v-align-middle .mr-2 }
Required if Not Inherited
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View Full MSU Documentation for Element →](/metadata-documentation/metadata/element/origin-info/#date)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- Populate the appropriate date columns for each item
  - Columns containing date fields must be grouped together
  - The first column in the group must be **originInfo_datetype**
  - Each instance of **originInfo_datetype** triggers the creation of a new date
  - Columns relevant to a single date or a date range should follow **originInfo_datetype**
  - Each date must include a year
  - If the date is not a valid date, the information will import as free text rather than encoded
    - Examples of invalid dates include dates that are in the future (e.g., the year `2026`) and dates that do not exist in the calendar (e.g., `1876-02-31`)
- If you are working with items that have multiple dates, discuss with the [Manager, Metadata Services](/metadata-documentation/contact/), before proceeding further

### Note
{: .d-inline .v-align-middle .mr-2 }
[View Full MSU Documentation for Element →](/metadata-documentation/metadata/element/note/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- Populate a **note** and **note_type** column for each item
  - See the [Note Type](/metadata-documentation/metadata/element/note/#type) attribute for a link to a list of note types
  - Only one note can be added during a CSV import

### Parent Record
{: .d-inline .v-align-middle .mr-2 }
Required if Not Specified in CSV Import Form
{: .d-inline .v-align-middle .label .label-blue .mx-1 }

- Populate a **parent_uuid** column to indicate the [UUID](/metadata-documentation/resources/glossary/#universally-unique-identifier) of the parent collection or container record where each item should be located
  - Providing parent records in the CSV is required when importing items into different locations, such as different containers within a parent collection
  - Parent records must already exist within MMS before the CSV import
- If there is no **parent_uuid** column in your CSV file, you must enter the UUID of the parent collection or container record in the upload form under **Step 3: Enter Parent UUID**