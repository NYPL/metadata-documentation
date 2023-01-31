---
layout: page
title: Name
permalink: /metadata/element/name/
parent: By Element
grand_parent: MMS › Metadata
nav_exclude: true
nav_order: 6
---

{: .highlight-title }
> 🚧 Under Construction
>
> This page is still being developed. Links to legacy documentation may appear to facilitate our migration process. [Contact us](/metadata-documentation/contact/) with any questions or feedback.

# Name
{: .d-inline .v-align-middle .no_toc .mr-2 }
Repeatable
{: .d-inline .v-align-middle .label .label-green .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/name.html)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

The name of a person, organization, or event (conference, meeting, etc.) associated with the resource
{: .d-block .mt-2 .fs-6 .fw-300 }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Purpose
- To record a person, organization, or event associated with the creation or production of a resource

## Guidelines
- Use the **Name** element only for people, organizations, or events associated with the creation or production of the resource or part of the resource
    - See [Subject › Name](/metadata-documentation/metadata/element/subject/#name) when the content of the resource is _about_ a person, organization, or event

## Subelements

---

### Name
{: .d-inline .v-align-middle .mr-2 }
Recommended if Applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/name.html)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_The name of a person, organization, or event (conference, meeting, etc.) associated with the resource_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
-   It is strongly recommended to always begin with an **Authority data search** as use of an authority with a URI is required if one exists
    - Select the radio button for **Authority data search**
    - Click **Select from controlled terms**
    - Look up the name, organization, or event you wish to add in the search box
    - To verify a result is correct, click the linked **Authorized Term** to view the authority record on the Library of Congress site
    - Once you have confirmed the correct result, click **Use this term**
    - Entering authorities using the Authority data search automatically populates Type, Authority, and Value URI
    - If no results appear to be correct, try adjusting your search terms or search directly on the [Library of Congress Linked Data Service](https://id.loc.gov/) website
        - MMS only periodically updates the results that appear within the Authority data search, so sometimes names will be present in [Library of Congress Linked Data Service](https://id.loc.gov/) that are not yet in MMS
        - Search the [LC Name Authority File (LCNAF)](https://id.loc.gov/authorities/names.html) first as most authorities for the **Name** element will appear in that catalog
        - If you receive no results in LCNAF, search the [LC Subject Headings (LCSH)](https://id.loc.gov/authorities/subjects.html).
        - If the authority you wish to use appears on the [Library of Congress Linked Data Service](https://id.loc.gov/), but not within MMS, follow the instructions below for adding a free text name
- If there is no Library of Congress Authority available via the **Authority data search**, select the radio button for **Free text**
    -   Search for the Name using the [LCNAF](https://id.loc.gov/authorities/names.html) or [LCSH](https://id.loc.gov/authorities/subjects.html)
        -   If the authority exists in LCNAF/LCSH... [TK]
-   Search for the Name using [VIAF](https://viaf.org/)
    -   If the authority exists in VIAF... [TK]
-   If the person, organization, or event does not have an authority record in LCNAF, LCSH, or VIAF, manually enter the name according to the according to the relevant [content standard](/metadata-documentation/metadata/guidelines/#content-standards)
- The order of preference for values for name authorities is 
    - LC Name Authority File (LCNAF) or LC Subject Headings (LCSH)
    - Virtual International Authority File (VIAF)
    - Free text
- See [MARC 100](https://www.loc.gov/marc/bibliographic/bd100.html), [MARC 110](https://www.loc.gov/marc/bibliographic/bd110.html), and [MARC 111](https://www.loc.gov/marc/bibliographic/bd111.html)

---

### Type
{: .d-inline .v-align-middle .mr-2 }
Required if Free Text
{: .d-inline .v-align-middle .label .label-blue .mx-1 }

#### Guidelines
{: .no_toc }
- Entering authorities using the Authority data search automatically populates Type
- If you are manually entering an authority from LCNAF, LCSH, or VIAF, you can find information about which Type to select on the page for that authority
- If no authority exists and you are entering a name with free text, you must decide which Type is appropriate
- Select the appropriate Type from the dropdown
    - The options are personal, corporate, conference, or family
- See [OCLC Access Points](https://www.oclc.org/bibformats/en/accesspoints.html)

---

### Authority
{: .d-inline .v-align-middle .mr-2 }
Required if Free Text and Applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }

#### Guidelines
{: .no_toc }
- Entering authorities using the Authority data search automatically populates Authority
- If you are entering an authority from LCNAF, LCSH, or VIAF, select the respective choice from the dropdown. The options are LC/NACO Authority File (LCNAF), Library of Congress subject headings, and VIAF
- If no authority exists and you are entering a name with free text, leave this blank

---

### Value URI
{: .d-inline .v-align-middle .mr-2 }
Required if Free Text and Applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }

#### Guidelines
{: .no_toc }
- Entering authorities using the Authority data search automatically populates Value URI
- Enter here the URI for the authority
- For LCNAF and LCSH, the URI can be found…
- For VIAF, the URI can be found…
- If no authority exists and you are entering a name with free text, leave this blank

---

### Role
{: .d-inline .v-align-middle .mr-2 }
Required if Applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/name.html#role)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_Designates the relationship (role) of the entity to the resource described in the record_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Every instance of a **Name** element requires a role be selected from the dropdown
- If the role is unknown, use Creator for the primary name…
- Use Contributor for additional names with unknown roles…
- See [MARC Code List for Relators](https://www.loc.gov/marc/relators/) and [Personal Names-General Information $e](https://www.loc.gov/marc/bibliographic/bdx00.html)
- To include multiple roles for a name, repeat the name in a new Name field for each role

---

### Affiliation
{: .d-inline .v-align-middle .mr-2 }
Do Not Use
{: .d-inline .v-align-middle .label .label-red .mx-1 }

---

## Attributes

---

### Primary
{: .d-inline .v-align-middle .mr-2 }
Required if Applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/attributes.html#usage)
{: .d-inline .v-align-middle .text-zeta .ml-2 }
_Used for a repeated element to declare that a particular instance of the element is most important_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Check **Primary** for <u>one</u> **Name** element if more than one **Name** element exists for a record

---

## See Also
- [Top-level Element: &lt;name&gt;](https://www.loc.gov/standards/mods/userguide/name.html) for official MODS documentation from the Library of Congress