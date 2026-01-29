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

## Research Catalog

### View MARC in Research Catalog
At the bottom of a record in the Research Catalog, click the link that says **View marc record ›**
_or_
Append `/marc` to the end of a Research Catalog record URL, e.g.: <a href="https://www.nypl.org/research/research-catalog/bib/b11599430/marc"><tt>https://www.nypl.org/research/research-catalog/bib/b11599430<span style="background: #ffffcc; border: 1px solid #5c5962;">/marc</span></tt></a>

## Legacy Catalog

### View MARC in Legacy Catalog
Place an `x` between `/` and `record` in a Legacy Catalog record URL, e.g.: <a href="https://legacycatalog.nypl.org/xrecord=b21530562~S1"><tt>https://legacycatalog.nypl.org/<span style="background: #ffffcc; border: 1px solid #5c5962;">x</span>record=b21530562~S1</tt></a>

{: .warning-title }
> Known Issue
>
> Certain browsers such as Google Chrome and Microsoft Edge are unable to render the MARC record in an easily readable format. Using Firefox is recommended.
> <small><br>Last checked January 2025</small>

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

### Library of Congress Identifier → Library of Congress Label
Replace `A2` with the cell containing the Library of Congress identifier
```
=INDEX(IMPORTXML("http://id.loc.gov/authorities/names/"&A2, "//meta[@name='dc.subject']/@content"), 2)
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

## OpenRefine

### Fetching Data from VIAF
1. Prepare a column in OpenRefine containing VIAF identifiers
1. In the header of a column containing VIAF identifiers, navigate to **▼** › **Add column by fetching URLs…**
1. In the prompt, enter a **New column name**, paste the below expression in the **Expression** field, and click the **OK** button
    ```
    "http://viaf.org/viaf/" + value + "/viaf.json"
    ```
1. Allow time for OpenRefine to fetch the JSON data
    1. Progress will be indicated by a message at the top of the screen

#### Fetching Redirected VIAF Identifiers
1. Follow the steps to [fetch data from VIAF](#fetching-data-from-viaf)
1. In the header of a column containing VIAF JSON, navigate to **▼** › **Add column based on this column…**
1. In the prompt, enter a **New column name**, paste the below expression in the **Expression** field, and click the **OK** button
    ```
    value.parseJson().redirect.directto
    ```
1. Optional: To facet your data to display only rows with redirects:
    1. In the header of the newly created column, navigate to **▼** › **Facet** › **Customized facets** › **Facet by blank (null or empty string)**
    1. In the **Facet / Filter** tab in the left column of OpenRefine, find the facet corresponding to the newly created column and select **false**

#### Fetching Library of Congress Identifiers from VIAF
1. Follow the steps to [fetch data from VIAF](#fetching-data-from-viaf)
1. In the header of a column containing VIAF JSON, navigate to **▼** › **Add column based on this column…**
1. In the prompt, enter a **New column name**, paste the below expression in the **Expression** field, and click the **OK** button
    ```
    value.parseJson().sources.source.find(/"LC\|([^"]+)"/)[0].replace("\"", "").split("|")[1].replace(" ", "")
    ```
1. Optional: To facet your data to display only rows with Library of Congress identifiers:
    1. In the header of the newly created column, navigate to **▼** › **Facet** › **Customized facets** › **Facet by blank (null or empty string)**
    1. In the **Facet / Filter** tab in the left column of OpenRefine, find the facet corresponding to the newly created column and select **false**

{: .note }
This same technique can be used to retrieve additional identifiers from VIAF by replacing `LC` with the code that corresponds to the respective [authority source code](https://www.oclc.org/developer/api/oclc-apis/viaf/authority-cluster.en.html#:~:text=Authority%20Source%20Codes).

## See Also
- [MMS Database and SQL Queries 🔒](https://github.com/NYPL/metadata-tools/tree/master/_mms-database-and-sql-queries) for example SQL queries, navigation information, and quick reference
- [Wikidata:WikiProject New York Public Library/Queries](https://www.wikidata.org/wiki/Wikidata:WikiProject_New_York_Public_Library/Queries) for reusable SPARQL queries for Wikidata
- [Regex Resources for Catalogers and Others in the Library](https://ruthtillman.com/post/regex-catalogers/) for an overview of Regular Expressions for a library audience
- [BenCollins: Spreadsheets](https://benlcollins.com/spreadsheets) for scripts and templates that can be used when working in Google Sheets
    - [VLOOKUP Function in Google Sheets: The Essential Guide](https://benlcollins.com/spreadsheets/vlookup-function/)
    - [Applying Conditional Formatting Across An Entire Row In Google Sheets](https://www.benlcollins.com/spreadsheets/conditional-formatting-entire-row/)