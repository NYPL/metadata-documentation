---
layout: page
title: Origin Info
permalink: /metadata/element/origin-info/
parent: By Element
grand_parent: MMS › Metadata
nav_exclude: true
nav_order: 5
---

# Origin Info
{: .d-inline .v-align-middle .no_toc .mr-2 }
Required
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
Repeatable
{: .d-inline .v-align-middle .label .label-green .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/origininfo.html)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

Information about the origin of the resource, including place of origin or publication, publisher/originator, and dates associated with the resource
{: .d-block .mt-2 .fs-6 .fw-300 }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Purpose
- To allow end users to discover resources by date
- To provide context regarding the publication and origination of the material
- To be used by [Copyright and Information Policy](/metadata-documentation/resources/glossary/#copyright-and-information-policy) to make copyright determinations and to apply appropriate rights profiles in MMS

## Guidelines
- See [subelements](#subelements)

## Subelements

---

### Date
{: .d-inline .v-align-middle .mr-2 }
Required
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
Repeatable
{: .d-inline .v-align-middle .label .label-green .mx-1 }

_The date of creation of the resource_ <a href="https://www.loc.gov/standards/mods/userguide/origininfo.html#datecreated" style="margin-left: 10px;"><small>View MODS Documentation for **Date created** →</small></a>
{: .d-block .mt-2 .mb-1 }
or
{: .text-delta .my-0 .py-0 }
_The date that the resource was published, released, or issued_ <a href="https://www.loc.gov/standards/mods/userguide/origininfo.html#dateissued" style="margin-left: 10px;"><small>View MODS Documentation for **Date issued** →</small>
{: .d-block .mt-1 }

#### Guidelines
{: .no_toc }

- Date is a required element
  - If no date can be found, you must estimate a date or date range (i.e. decade or century)
  - If a container or item record has a narrower date than is inherited from a higher-level collection or container, disinherit the **Origin Info** element and add the narrower date to a given container or item
- Select the appropriate date **Type** from the dropdown
  - Use **Date created** for most unpublished materials
  - Use **Date issued** for most published materials
  - Do not use **Date captured**, **Copyright date**, or **Other date**
    - Dates related to ownership, copyright, gift, etc. can be expressed as free text in a [**Note**](/metadata-documentation/metadata/element/note/) element with the [**Type**](/metadata-documentation/metadata/element/note/#type) "date" with a prefix for context, e.g. "Gift: 1937"
- Add the relevant date(s) encoded as a **Single date** or **Date range**
  - Select **Single date** if you know the point in time a resource was created or issued
    - If adding more than one **Single date** field, select the most relevant encoded date as **Key date**
  - Select **Date range** if the date of a resource is provided as range or you are uncertain about the point in time a resource was created or issued
    - Enter a range of dates (no matter how broad) to narrow down the date, e.g. to express that a resource was created in the 1920s, select **Date range**, enter a **Start date** of 1920 and an **End date** of 1929 and select **approximate** for the **Qualifier** of both fields
    - Indicate the **Start date** of the range as the **Key date**
  - Enter the most specific date known in the **Year**, **Month**, and **Day** fields
    - **Year** is required, while **Month** and **Day** are optional
    - By default all date(s) are set to **CE** to indicate the date is common era
    - If a date is before the common era (BCE), toggle the radio button to **BCE**
  - Select a **Qualifier** if appropriate for any dates to indicate that they are approximate, inferred, or questionable
    - Select **approximate** for uncertain date ranges and for "circa" dates that are not guaranteed to be exact
    - Select **inferred** for known dates not transcribed directly from a resource
    - Select **questionable** for questionable dates
- Generally, dates should not be recorded free text using the **Text (for non-Gregorian calendar dates)** option
  - Non-Gregorian dates, decades, and seasons should be converted to their corresponding Gregorian date/range
    - Add a [**Note**](/metadata-documentation/metadata/element/note/) element with the [**Type**](/metadata-documentation/metadata/element/note/#type) "date" with a prefix for context that specifies the original calendar type, date, and date type, e.g. "Date issued: 1003 (Islamic calendar)" or "Date created: 1743 (Julian calendar)"
  - "Circa" or "approximate" dates can be recorded as an encoded date/range with the use of the relevant **Qualifier**
  - Dates provides as seasons, can be recorded using **Date range** to record the range of months that correspond to that season
    - Seasons in the Northern Hemisphere:
      - Winter: record month range 01–03
      - Spring: record month range 04–06
      - Summer: record month range 07–09
      - Fall: record month range 10–12
    - Seasons in the Southern Hemisphere:
      - Winter: record month range 07–09
      - Spring: record month range 10–12
      - Summer: record month range 01–03
      - Fall: record month range 04–06
    - Add a [Note](/metadata-documentation/metadata/element/note/) element with the [Type](/metadata-documentation/metadata/element/note/#type) "date" with a prefix for context that specifies the original calendar type, date, and date type, e.g. "Date issued: Summer 1968"
  - If you believe there to be a reason to record a date as **Text (for non-Gregorian calendar dates)**, discuss with the [Interim Manager, Metadata Services](/metadata-documentation/contact/), before proceeding further
- For reprints, add the date of the reprint in the **Date issued field**, not the date of the original item's creation or issuance
  - You may put the original print date in a [**Note**](/metadata-documentation/metadata/element/note/) element with the [**Type**](/metadata-documentation/metadata/element/note/#type) "date" with a prefix for context, e.g. "Original: 1920"

---

### Place
{: .d-inline .v-align-middle .mr-2 }
Repeatable
{: .d-inline .v-align-middle .label .label-green .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/origininfo.html#place)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_A place associated with the event_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Provide a free text description of the place the resource was created or issued
  - Syntax of a **Place** subelement that has been [imported](/metadata-documentation/workflows/importing/) or transcribed directly from the source can remain as-is
    - See [content standard](/metadata-documentation/metadata/guidelines/#content-standards)
  - If the place is not imported or transcribed but still can be determined, add a **Place** subelement with the authorized heading for the place as it appears in a controlled vocabulary, listed here in order of preference:
    - [Library of Congress Name Authority File (LCNAF) - Geographic](https://id.loc.gov/search/?q=rdftype:Geographic\&q=cs%3Ahttp%3A%2F%2Fid.loc.gov%2Fauthorities%2Fnames)
    - [Library of Congress Subject Headings (LCSH) - Geographic](https://id.loc.gov/search/?q=\&q=memberOf%3Ahttp%3A%2F%2Fid.loc.gov%2Fauthorities%2Fsubjects%2Fcollection_GeographicSubdivisions\&q=cs%3Ahttp%3A%2F%2Fid.loc.gov%2Fauthorities%2Fsubjects)
  - If the place is not imported, transcribed, or findable in a controlled vocabulary, add a **Place** subelement with the place name spelled out in its fullest form
- Remove brackets enclosing the entirety of the **Place** subelement
  - If brackets indicated the **Place** was devised and not transcribed from the resource, check the **Supplied** box
- Leave the **Value type** dropdown as **text**
- For places depicted in the content of the resource, use [**Geographic Subject**](/metadata-documentation/metadata/element/subject/#geographic)

---

### Publisher
{: .d-inline .v-align-middle .mr-2 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/origininfo.html#publisher)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_The name of the entity that published, printed, distributed, released, issued, or produced the resource_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Provide a free text description of who published the resource
  - Choice and format of the **Publisher** subelement should be governed by the relevant [content standard](/metadata-documentation/metadata/guidelines/#content-standards)
- Do not include brackets in the **Publisher** subelement
  - Check the **Supplied** box  if the **Publisher** was not directly transcribed from the resource but instead provided by the person creating the description
- Do not add the name of the institution responsible for digitizing and delivering online a previously published resource
  - If necessary to add, this information can be input in a [**Note**](/metadata-documentation/metadata/element/note/) element

---

### Edition
{: .d-inline .v-align-middle .mr-2 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/origininfo.html#edition)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_Information identifying the version of the resource_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Transcribe any available edition information using the relevant [content standard](/metadata-documentation/metadata/guidelines/#content-standards)
- Do not include brackets in the **Edition** subelement
- Check the **Supplied** box if the **Edition** was not directly transcribed from the resource but instead provided by the person creating the description

---

### Issuance
{: .d-inline .v-align-middle .mr-2 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/origininfo.html#issuance)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_A term that designates how the resource is issued_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- This subelement is not widely used at the present time, but you can select **serial** if appropriate

---

## Attributes

---

### Supplied
{: .d-inline .v-align-middle .mr-2 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/attributes.html#supplied)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_Indicates whether the content of the element has been supplied from external sources, or from a source other than the ones prescribed by the content standard used_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Refer to [**Place**](#place), [**Publisher**](#publisher), and [**Edition**](#edition) for guidelines on when to check the **Supplied** box in those respective subelements

---

## See Also
- [Top-level Element: &lt;originInfo&gt;](https://www.loc.gov/standards/mods/userguide/origininfo.html) for official MODS documentation from the Library of Congress