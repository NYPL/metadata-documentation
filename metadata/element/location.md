---
layout: page
title: Location
permalink: /metadata/element/location/
parent: By Element
grand_parent: MMS › Metadata
nav_exclude: true
nav_order: 16
---

# Location
{: .d-inline .v-align-middle .no_toc .mr-2 }
Required
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/location.html)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

The institution or repository holding the resource, the physical location of the resource, and/or the electronic location for a digital resource in the form of a URL
{: .d-block .mt-2 .fs-6 .fw-300 }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Purpose
- To help users and staff locate the original physical object
- To help users and staff direct questions about the object to the appropriate division

## Guidelines
- See [subelements](#subelements)

## Subelements

---

### Repository
{: .d-inline .v-align-middle .mr-2 }
Required
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/location.html#physicallocation)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_The institution or repository that holds the resource or where it is available_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Select New York Public Library
    - If the resource is not one held by the New York Public Library, discuss with the [Interim Manager, Metadata Services](/metadata-documentation/contact/) before proceeding further

---

### NYPL Division/Collection
{: .d-inline .v-align-middle .mr-2 }
Required
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/location.html#physicallocation)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_The Library division or collection that holds the resource or where it is available_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Select the Library division that owns the resource from the dropdown list
    - Provide the name of the owning division, rather than the exact physical location of the original materials, as physical location may change over time or may only be known by division staff
    - If consulting a MARC record to determine division:
        - Find the location code nested within `<FIXFLD><FIXVALUE>` in the [MARC XML](/metadata-documentation/resources/tips-tricks/#view-marc-in-legacy-catalog) and look up the corresponding label in [Sierra codes/locations 🔒](https://docs.google.com/spreadsheets/d/1E8Dbd8M5OotQfGaKjL5cLKlyex5g8D1KBeZeArJtcuU/edit#gid=1867405302)
        - In cases where the MARC XML indicates multiple locations (`<FIXVALUE>multi</FIXVALUE>`), locate the record in [Sierra](/metadata-documentation/resources/glossary/#sierra) and consult the **Summary** tab to determine which location corresponds to the relevant item's [Call number / Shelf Locator](#call-number--shelf-locator)
- Do not use the following values unless you have discussed doing so with the [Interim Manager, Metadata Services](/metadata-documentation/contact/)
    - Children's Center at 42nd St
    - Comm, Marketing, and Business Dev
    - Dorothy and Lewis B. Cullman Center for Scholars and Writers
    - External, not NYPL
    - No Division
    - Reference and Research Services
    - Reserve Film and Video Collection
    - Unknown
- Choose only one NYPL division
    - If a source catalog record for a resource describes materials owned by multiple divisions, this generally warrants separate records for each division
    - If you believe there to be a reason to create a record in MMS that corresponds to multiple NYPL divisions, discuss with the [Interim Manager, Metadata Services](/metadata-documentation/contact/), before proceeding further

---

### Call number / Shelf Locator
{: .d-inline .v-align-middle .mr-2 }
Required
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/location.html#shelflocator)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_Shelfmark or other shelving designation that indicates the location identifier for a copy_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Add the call number or shelf locator into the free-text field if one is available
    - Each individual item might not have its own unique call number/shelf locator and these are often inherited
    - When importing descriptive information from a finding aid, box and folder information should be moved to an [**Note**](/metadata-documentation/metadata/element/note/) field with **admin** selected as the type

---

## See Also
- [Top-level Element: &lt;location&gt;](https://www.loc.gov/standards/mods/userguide/location.html) for official MODS documentation from the Library of Congress
- [Sierra codes/locations 🔒](https://docs.google.com/spreadsheets/d/1E8Dbd8M5OotQfGaKjL5cLKlyex5g8D1KBeZeArJtcuU/edit#gid=1867405302) for a list of Library location codes and their corresponding label to assist in determining the **NYPL Division/Collection**