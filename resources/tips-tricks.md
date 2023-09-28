---
layout: page
title: Tips & Tricks
permalink: /resources/tips-tricks/
parent: Resources
nav_order: 5
---

# Tips & Tricks
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Legacy Catalog

### View MARC in Legacy Catalog
Place an `x` in front of a record URL, e.g.: <a href="https://legacycatalog.nypl.org/xrecord=b21530562~S1"><tt>https://legacycatalog.nypl.org/<span style="background: #ffffcc; border: 1px solid #5c5962;">x</span>record=b21530562~S1</tt></a>

## Archives Portal

### View XML in Archives Portal
Add `.xml` after a collection URL, e.g.: <a href="https://archives.nypl.org/brg/19343.xml"><tt>https://archives.nypl.org/brg/19343<span style="background: #ffffcc; border: 1px solid #5c5962;">.xml</span></tt></a>

{: .note }
Only EAD-encoded finding aids will have XML that contains the full finding aid's content.

## Metadata Management System

### View MODS XML
1. On the **Descriptive metadata** tab of a Collection, Container, or Item record, use either method:
    1. Click **Preview complete MODS record** under the Descriptive Metadata Heading 
    1. Click **XML MODS export**
        1. In the popup prompt, type ```admin``` as the username and ```password``` as the password

## Google Sheets

### Division Acronym → MSU Liaison
Replace `A2` with the cell containing the division's acronym
```
=IFERROR(vlookup(A2,IMPORTRANGE("https://docs.google.com/spreadsheets/d/1P-YDJigon640fTCLP4Ig4-zmzqrX88v5M24ShuxFNVY/edit#gid=0","Metadata Liaisons and Contacts!A3:F37"),6,false),)
```

### Sierra Location Code → Location Name
Replace `A2` with the cell containing the Sierra location code
```
=IFERROR(vlookup(A2,IMPORTRANGE("https://docs.google.com/spreadsheets/d/1E8Dbd8M5OotQfGaKjL5cLKlyex5g8D1KBeZeArJtcuU/edit#gid=1867405302","sierra-codes-locations!F2:G2889"),2,false))
```

### Full bnumber → Short bnumber
Replace both instances of `A2` with the cell containing the full bnumber
```
=LEFT(A2,(SUM(LEN(A2)-1)))
```

### Import List of Relator Name Elements
Use this function to import relator names into a standalone tab in your spreadsheet for data validation
```
=IMPORTRANGE("https://docs.google.com/spreadsheets/d/1lG2UypYYLTSefUWsTv2w8qLfm6tP-gflJ7VWr3QZIM0/edit#gid=0","name element!A2:A268")
```

### Check if URL Contains DC-Related Domains
Replace `A2` with the cell containing the URL
```
=IF(REGEXMATCH(A2, "digital.nypl.org|digilib.nypl.org|llink.nypl.org|digitalgallery.nypl.org|nypl.org/digital|link.nypl.org|purl.nypl.org|digitalcollections.nypl.org"), TRUE, FALSE)
```

### Add Thumbnail Using Image ID
Replace `A2` with the cell containing the Image ID
```
=IMAGE(https://images.nypl.org/index.php?t=w&id=A2)
```

### Copy Cell Above If Cell Is Blank
```
=INDIRECT(ADDRESS(ROW()-1,COLUMN()))
```

### Count Occurrences in Row
Replace `A$2:A` with the range and `A2` with the cell containing the string you wish to count

```
=COUNTIF(A$2:A,A2)
```

### Highlight Duplicate Cell Data in Row
1. Select the column you'd like to highlight duplicate cell data
1. From the **Format** menu, select **Conditional Formatting** and the **Conditional format rules** menu will open on the right side of the window
1. In the **Format cells if…** dropdown menu, select **Custom formula is** and paste the below formula in the **Value or Formula** field, replacing the three occurrences of `A` with the letter of the column that you'd like to highlight duplicate cell data, and click the **Done** button to apply

```
=COUNTIF(A:A,A2)>1
```

### Make Cells with URLs Clickable
1. Navigate to **Edit** › **Find and replace**
1. Enter **http** in both the **Find** and **Replace with** fields
1. Click **Replace all** twice

## See Also
- [MMS SQL Queries 🔒](https://github.com/NYPL/metadata-tools/tree/master/_mms-sql-queries) for reusable SQL queries for MMS
- [Wikidata:WikiProject New York Public Library/Queries](https://www.wikidata.org/wiki/Wikidata:WikiProject_New_York_Public_Library/Queries) for reusable SPARQL queries for Wikidata
- [BenCollins: Spreadsheets](https://benlcollins.com/spreadsheets) for scripts and templates that can be used when working in Google Sheets
    - [VLOOKUP Function in Google Sheets: The Essential Guide](https://benlcollins.com/spreadsheets/vlookup-function/)
    - [Applying Conditional Formatting Across An Entire Row In Google Sheets](https://www.benlcollins.com/spreadsheets/conditional-formatting-entire-row/)