---
layout: page
title: Name
permalink: /metadata/element/name/
parent: By Element
grand_parent: MMS › Metadata
nav_exclude: true
nav_order: 6
---

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
- Use the **Name** element only for people, organizations, families, or events associated with the creation or production of the resource or part of the resource
    - See [**Subject**](/metadata-documentation/metadata/element/subject/) type **Name** when the content of the resource is about a person, organization, or event
- Use of an authority with a URI is required, if one exists
- If importing metadata, pay special attention to **Name** elements to ensure they are consistently imported with the appropriate [Role](#Role)
    - Whether **Name** elements are imported into MMS from a [finding aid](h/metadata-documentation/workflows/import/#importing-finding-aids) depends on the level of description that exists in the [Archives Portal](/metadata-documentation/resources/glossary/#archives-portal)
    - If **Name** elements are missing, it may be helpful to reference the **Added Author** fields in corresponding library catalog record (linked as **Call number** from the Archives Portal finding aid)

## Subelements

---

### Name Part
{: .d-inline .v-align-middle .mr-2 }
Required if Name Element Present
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/name.html#namepart)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_The individual parsed parts that together make up the full name_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- The **Name Part** subelement appears as an unlabeled text field in the **Name** element
- When adding a new **Name** element, start by searching the MMS authorities module
    - Select the radio button for **Authority data search**
    - Click **Select from controlled terms** to bring up the authorities module
    - Look up the name you wish to add in the search box
        - For personal names, search in indirect order (i.e. "last name, first name")
    - The order of preference for names are:
        - LC Name Authority File (LCNAF)
        - Virtual International Authority File (VIAF)
        - Free text
    - To verify a result is correct, click the linked **Authorized Term** to view the corresponding record in the source authority
    - Once you have confirmed the correct result, click the **Use this term button**
    - Selecting a name from the MMS authorities module automatically populates the **Name Part** subelement and the **Type**, **Authority**, and **Value URI** attributes
- If you are not receiving the result you expect by searching the MMS authorities module, try searching the [Library of Congress Linked Data Service](https://id.loc.gov/)
    - It is possible that the name you are searching exists in the [Library of Congress Linked Data Service](https://id.loc.gov/) but does not exist in the MMS authorities module
    - This can occur because the MMS authorities module data is only periodically updated and is therefore out of sync with the [Library of Congress Linked Data Service](https://id.loc.gov/)
    - In this case, follow the instructions below for adding a **Name** as free text
- If you are unable to find a name using the **Authority data search**, you may add it as free text
    - Select the radio button for **Free text**
    - If the authority exists in LCNAF but it is not appearing for selection from the MMS authorities module, input the LCNAF label manually
    - If the authority exists in VIAF:
        - Input the name as it been used in an NYPL catalog record
        - If no NYPL catalog record with that name exists, select and input a name string from VIAF that most closely adheres to <a href="#lc-name-guidelines">LC name formatting guidelines</a>
        - If none of the VIAF labels meet this criteria, construct and input the name according to <a href="#lc-name-guidelines">LC name formatting guidelines</a>
    - If a name does not appear in LC or VIAF, construct and input the name according to <a href="#lc-name-guidelines">LC name formatting guidelines</a>
    - Select the appropriate [**Type**](#type) attribute from the dropdown
    - For names from LCNAF and VIAF, select the appropriate [**Authority**](#authority) from the dropdown, and add a properly formatted [**Value URI**](#value-uri)
    - Select the appropriate [**Role**](#role) from the dropdown
- <a name="lc-name-guidelines"></a>See the following pages for LC name formatting guidelines:
    - [MARC 100](https://www.oclc.org/bibformats/en/1xx/100.html) for personal name and family names type
        - [Personal name constructions, examples](https://sites.google.com/a/bookops.org/cataloging/naco/rda-personal-names/personal-name-constructions-examples) for examples of constructing personal names created by BookOps
    - [MARC 110](https://www.oclc.org/bibformats/en/1xx/110.html) for corporate name type
    - [MARC 111](https://www.oclc.org/bibformats/en/1xx/111.html) for conference name type

---

### Role
{: .d-inline .v-align-middle .mr-2 }
Required if Name Element Present
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/name.html#role)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_Designates the relationship (role) of the entity to the resource described in the record_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Every **Name** element requires a **Role** be selected from the dropdown
- To include multiple roles for one name, create a new **Name** element for each **Role**
- Use the most precise known **Role** known (e.g., **Author** or **Addressee** rather than the more general role **Correspondent**)
- Use **Contributor** for **Name** elements where the **Role** is unknown and/or can not be determined
- For [finding aid imports](/metadata-documentation/workflows/import/#importing-finding-aids), ensure that the archives collection creator listed the Archives Portal is present as a **Name** element with the role **Creator**
    - If there are multiple **Name** elements, ensure that the **Name** with the **Creator** role is marked [Primary](#primary)
See [MARC Code List for Relators](https://www.loc.gov/marc/relators/) and [Personal Names-General Information $e](https://www.loc.gov/marc/bibliographic/bdx00.html)

---

### Affiliation
{: .d-inline .v-align-middle .mr-2 }
Do Not Use
{: .d-inline .v-align-middle .label .label-red .mx-1 }

---

## Attributes

---

### Type
{: .d-inline .v-align-middle .mr-2 }
Required if Name Element Present
{: .d-inline .v-align-middle .label .label-blue .mx-1 }

#### Guidelines
{: .no_toc }
- Adding a **Name** using the authorities module automatically populates **Type**
- If you are inputting a name as free text, select the appropriate **Type** from the dropdown
    - The options are **personal**, **corporate**, **conference**, or **family**
    - If you are manually entering an authority from LCNAF or VIAF, you can find information about which **Type** to select on the page for that authority
- See [OCLC Access Points](https://www.oclc.org/bibformats/en/accesspoints.html)

---

### Authority
{: .d-inline .v-align-middle .mr-2 }
Required if Applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/attributes.html#authority)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_The name of an authoritative list of terms for an element whose values are controlled_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Adding a **Name** using the authorities module automatically populates **Authority**
- If you are entering a free text name from LCNAF or VIAF, select the appropriate **Authority** from the dropdown
    - The options are **LC Name Authority File (LCNAF)** and **Virtual International Authority File (VIAF)**
- If you are entering a free text name with no corresponding authority, leave **Authority** blank

---

### Value URI
{: .d-inline .v-align-middle .mr-2 }
Required if Applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/attributes.html#valueURI)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_When the authoritative list is a linked data vocabulary, @valueURI can point directly to the term_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Adding a **Name** using the authorities module automatically populates **Value URI**
- If you are entering a free text name from LCNAF or VIAF, manually add the [Uniform Resource Identifier](/metadata-documentation/resources/glossary/#uniform-resource-identifier) (URI) to the **Value URI** field
    - For LCNAF and LCSH, the URI is the first value listed in the URI(s) section
        - Example: [`http://id.loc.gov/authorities/names/n88156657`](https://id.loc.gov/authorities/names/n88156657.html#:~:text=http%3A//id.loc.gov/authorities/names/n88156657)
    - For VIAF, the URI is listed in the Permalink field, which is located just above the Preferred Forms section
        - Example: [`http://viaf.org/viaf/96605017`](https://viaf.org/viaf/96605017/#:~:text=http%3A//viaf.org/viaf/96605017)
- If you are entering a free text name with no corresponding authority, leave **Value URI** blank

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
- For [finding aid imports](/metadata-documentation/workflows/import/#importing-finding-aids) with multiple names, the **Name** with the role, **Creator**, should be marked **Primary**

---

## See Also
- [Top-level Element: &lt;name&gt;](https://www.loc.gov/standards/mods/userguide/name.html) for official MODS documentation from the Library of Congress
- [Personal name constructions, examples](https://sites.google.com/a/bookops.org/cataloging/naco/rda-personal-names/personal-name-constructions-examples) for examples of constructing personal names created by BookOps
