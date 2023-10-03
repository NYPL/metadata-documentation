---
layout: page
title: Subject
permalink: /metadata/element/subject/
parent: By Element
grand_parent: MMS › Metadata
nav_exclude: true
nav_order: 11
---

# Subject
{: .d-inline .v-align-middle .no_toc .mr-2 }
Repeatable
{: .d-inline .v-align-middle .label .label-green .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/subject.html)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

A term or phrase representing the primary topic(s) on which a work is focused
{: .d-block .mt-2 .fs-6 .fw-300 }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Purpose
- To allow users to filter and explore resources by topic, place, time period, name subject, and work subject

## Guidelines
- Generally, **Subject** elements will be imported (from catalog records, finding aids, or TMS records) or added by Metadata Services Unit (MSU) staff
  - At least one subject is recommended
  - Only add **Subject** elements if you are familiar with relevant guidelines
  - See [Library of Congress Subject Headings: Online Training](https://www.loc.gov/catworkshop/lcsh/index.html) and [Library of Congress Subject Headings Manual](https://www.loc.gov/aba/publications/FreeSHM/freeshm.html)
- Determine the appropriate method to add a subject based on whether you wish to add a new, distinct subject or a subdivision
  - To add a new, distinct subject as its own element, click **+ Subject** 
  - To add a subdivision to create a complex subject heading, click the relevant type link to the right of **Add** within an existing **Subject** element
- When adding a new **Subject** element, start by searching the MMS authorities module
  - Select the appropriate subject type (**Topical**, **Geographic**, **Temporal**, **Name**, **Title**, or **Occupation**) for each subject you enter
    - See [Subelements](#subelements) for guidelines for each subject type
  - Click **Select from controlled terms** to bring up the authorities module
  - Look up the subject you wish to add in the search box
    - The selected subject type will determine which **Authority** is searched, and consequently which terms are available
    - Reference relevant guidelines for the record's [division](https:///metadata-documentation/metadata/division/) and [material](https:///metadata-documentation/metadata/material/) to determine whether there is any relevant preference for terms from a particular **Authority**
  - To verify a result is appropriate, click the linked **Authorized Term** to view the corresponding record in the source **Authority**
    - Review the selected record to ensure the subject you are adding can be used as you intend, e.g. do not add subdivision as a main subject
  - Once you have confirmed the correct result, click the **Use this term** button in the **Action** column
  - Selecting a subject from the MMS authorities module automatically populates the [**Type**](#type) ****(where applicable), [**Authority**](#authority) and [**Value URI** ](#value-uri)attributes
- If you are not receiving the result you expect by searching the MMS authorities module, try searching the [Library of Congress Linked Data Service](https://id.loc.gov/)
  - It is possible that the subject you are searching exists in the [Library of Congress Linked Data Service](https://id.loc.gov/) but is not yet available or up-to-date in the MMS authorities module
  - This can occur because the MMS authorities module data is only periodically updated and therefore may out of sync with the current version of the [Library of Congress Linked Data Service](https://id.loc.gov/)
- If you are unable to find a subject using the **Authority data search**, you may add it as free text
  - If the authority exists in a particular vocabulary but it is not appearing for selection from the MMS authorities module, input the label, [**Authority**](#authority), and [**Value URI**](#value-uri) from LCSH or LCNAF manually
  - If you are uncertain of the subject type, either:
    - Review the **Instance Of** section of the subject authority
    - Open the **MARC/XML** (linked under **Alternate Formats**), and compare the number to tag of the authorized form to the numbers on the [MARC 21 Format for Authority Data](https://www.loc.gov/marc/authority/ad1xx3xx.html)

## Subelements

---

### Topic
{: .d-inline .v-align-middle .mr-2 }
Repeatable
{: .d-inline .v-align-middle .label .label-green .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/subject.html#topic)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_Used as the tag for any topical subjects that are not appropriate in the &lt;geographic&gt;, &lt;temporal&gt;, &lt;titleInfo&gt;, &lt;name&gt;, &lt;genre&gt;, &lt;hierarchicalGeographic&gt;, or &lt;occupation&gt; subelements, or where the type is unknown_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Use the **Topic** subelement of **Subject** when the content of a resource is not described by one of the other categories of subelements
- Searching the authorities module within a **Topical** subelement will return **Authorized Terms** from the following vocabularies, listed here in order of preference: 
  - [LC Subject Headings (LCSH)](https://id.loc.gov/authorities/subjects.html)
    - Prioritize for textual materials
  - [Thesaurus for Graphic Materials (TGM) ](https://www.loc.gov/pictures/collection/tgm/)
    - Prioritize for visual materials
  - [Library of Congress Genre/Form Terms (LCGFT) ](https://www.loc.gov/catdir/cpso/genreformgeneral.html)
    - Use only as a **Topic** subject element if term relates to what the resources is “of” or “about”
    - If the term describes the nature of the content or function of the resource, relocate the term to the [**Genre**](https:///metadata-documentation/metadata/element/genre/) element
- Do not select an **Authorized Term** from [Virtual International Authority File (VIAF)](https://viaf.org/)
- See [MARC 650](https://www.oclc.org/bibformats/en/6xx/650.html) and resources listed under [See Also](#see-also) for information on when and how to use **Topical** subject headings and subdivisions, including when it is appropriate to enter a term that does not appear in one of the vocabularies

---

### Geographic
{: .d-inline .v-align-middle .mr-2 }
Repeatable
{: .d-inline .v-align-middle .label .label-green .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/subject.html#geographic)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_Used for simple geographic subject terms_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Use the **Geographic** subelement of **Subject** when the content of the resource is _about_ a place
  - Geographic subjects are commonly used as subdivisions of **Topic** subjects
- Searching the authorities module within a **Geographic** subelement will return **Authorized Terms** from the following vocabularies, listed here in order of preference: 
  - [LC/NACO authority file (LCNAF)](https://id.loc.gov/authorities/names.html)
  - [LC Subject Headings (LCSH)](https://id.loc.gov/authorities/subjects.html)
- Do not select an **Authorized Term** from [Getty Thesaurus of Geographic Names (TGN)](https://www.getty.edu/research/tools/vocabularies/tgn)
- See [MARC 651](https://www.oclc.org/bibformats/en/6xx/651.html) and resources listed under [See Also](#see-also) for information on when and how to use **Geographic** subject headings and subdivisions, including when it is appropriate to enter a term that does not appear in one of the vocabularies

---

### Name
{: .d-inline .v-align-middle .mr-2 }
Repeatable
{: .d-inline .v-align-middle .label .label-green .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/subject.html#name)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_A name used as a subject_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Use the **Name** subelement of **Subject** when the content of the resource is _about_ a person, organization, or event
  - Use the top-level [**Name**](https:///metadata-documentation/metadata/element/name/) element when adding people, organizations, families, or events associated with the creation or production of the resource or part of the resource
  - For personal names, use indirect order (i.e. “last name, first name”)
- Searching the authorities module within a **Name** subelement will return **Authorized Terms** from the following vocabularies, listed here in order of preference:
  - [LC/NACO authority file (LCNAF)](https://id.loc.gov/authorities/names.html)
  - [LC Subject Headings (LCSH)](https://id.loc.gov/authorities/subjects.html)
  - [Virtual International Authority File (VIAF)](https://viaf.org/)
  - Free text
- See [MARC 600](https://www.oclc.org/bibformats/en/6xx/600.html), [MARC 610](https://www.oclc.org/bibformats/en/6xx/610.html), [MARC 611](https://www.oclc.org/bibformats/en/6xx/611.html) and resources listed under [See Also](#see-also) for information on when and how to use **Name** subject headings and subdivisions, including when it is appropriate to enter a term that does not appear in one of the vocabularies

---

### Title
{: .d-inline .v-align-middle .mr-2 }
Repeatable
{: .d-inline .v-align-middle .label .label-green .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/subject.html#titleinfo)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_A title used as a subject_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Use the **Title** subelement of **Subject** when the content of the resource is _about_ a titled work
- Searching the authorities module within a **Title** subelement will return **Authorized Terms** from the following vocabularies, listed here in order of preference:
  - [LC/NACO authority file (LCNAF)](https://id.loc.gov/authorities/names.html)
  - [LC Subject Headings (LCSH) ](https://id.loc.gov/authorities/subjects.html)
  - Free text
- See [Preferred Titles–General Information](https://www.oclc.org/bibformats/en/accesspoints/x30.html#subfielda) and resources listed under [See Also](#see-also) for information on when and how to use **Title** subject headings and subdivisions, including when it is appropriate to enter a term that does not appear in one of the vocabularies

---

### Occupation
{: .d-inline .v-align-middle .mr-2 }
Repeatable
{: .d-inline .v-align-middle .label .label-green .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/subject.html#occupation)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_An occupation described by the resource_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Use the **Occupation** subelement of **Subject** when the content of the resource is _about_ an occupation
- **Occupation** subelements of **Subject** are automatically added during [finding aid imports](https:///metadata-documentation/workflows/import/#importing-finding-aids) when **Occupation** subjects are present on the finding aid
  - See the [NYPL Archival Processing Manual](https://docs.google.com/document/d/1AD5DpkyzCEeBaBoAtAy71qo4tyabB2yy28xkkXx-P4s/edit#heading=h.9q8h9ik6hap8) for internal guidelines including that occupations be selected from the [ITOAMC list](https://folgerpedia.folger.edu/Index_terms_for_occupations_in_archival_and_manuscript_collections_\(ITOAMC\))
  - To map ITOAMC values, follow the order of preference for **Occupation** below
- Searching the authorities module within a **Occupation** subelement will return **Authorized Terms** from the following vocabularies, listed here in order of preference: 
  - [LC Subject Headings (LCSH)](https://id.loc.gov/authorities/subjects.html)
  - [Thesaurus for Graphic Materials (TGM)](https://www.loc.gov/pictures/collection/tgm/)
  - [Getty Art and Architecture Thesaurus (AAT)](https://www.getty.edu/research/tools/vocabularies/aat/)

---

### Temporal
{: .d-inline .v-align-middle .mr-2 }
Repeatable
{: .d-inline .v-align-middle .label .label-green .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/subject.html#temporal)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_Used for chronological subject terms or temporal coverage_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Use the **Temporal** subelement of **Subject** when the content of the resource is _about_ a time period, date, or event
  - **Temporal** subjects are often added as subdivisions of [**Topic**](#topic) or [**Geographic**](#geographic) subjects
- See resources listed under [See Also](#see-also) for information on when and how to use **Temporal** subject headings and subdivisions, including when it is appropriate to enter a term that does not appear in one of the vocabularies

---

## Attributes

---

### Type
{: .d-inline .v-align-middle .mr-2 }
Required if Applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }

_The type of name_{: .mt-2 }[View MODS Documentation for **Name › Type** →](https://www.loc.gov/standards/mods/userguide/name.html#type){: .d-inline .v-align-middle .text-zeta .ml-2 }

OR
{: .d-block .fs-2 }

_Identifies what type of title is recorded_{: .mt-2 }[View MODS Documentation for **Title › Type** →](https://www.loc.gov/standards/mods/userguide/titleinfo.html#type){: .d-inline .v-align-middle .text-zeta .ml-2 }

#### Guidelines
{: .no_toc }
- Appears only for **Name** and **Title** subjects
  - See [Name › Type](https:///metadata-documentation/metadata/element/name/#type) documentation for more information on name types
- Select the appropriate **Type**

---

### Authority
{: .d-inline .v-align-middle .mr-2 }
Required if Free Text and Applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/attributes.html#authority)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_The name of an authoritative list of terms for an element whose values are controlled_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Adding a **Subject** using the authorities module automatically populates **Authority**
- If you are inputting a subject subelement from LCNAF, LCSH, LCGFT, TGM, AAT or VIAF as free text, select the appropriate **Authority** from the dropdown

---

### Value URI
{: .d-inline .v-align-middle .mr-2 }
Required if Free Text and Applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/attributes.html#valueURI)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_When the authoritative list is a linked data vocabulary, @valueURI can point directly to the term_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Adding a **Subject** using the authorities module automatically populates **Value URI**
- If you are inputting a name from LCNAF or VIAF as free text, manually add the Uniform Resource Identifier (URI) to the **Value URI** field
  - For LCNAF, LCSH, LCGFT, and TGM, the URI is the first value listed as the **URI(s)**, e.g. [http://id.loc.gov/authorities/names/n88156657](https://id.loc.gov/authorities/names/n88156657.html#:~:text=http%3A//id.loc.gov/authorities/names/n88156657)
  - For VIAF, the URI is the value listed as the **Permalink**, e.g. [http://viaf.org/viaf/115297970](https://viaf.org/viaf/115297970/#:~:text=http%3A//viaf.org/viaf/115297970)
- For AAT, click **Semantic View** at the top of the record, and the URI is the value listed as the **Source** just below the AAT term, e.g. [http://vocab.getty.edu/aat/300025427](http://vocab.getty.edu/aat/300025427#:~:text=http%3A//vocab.getty.edu/aat/300025427)

---

## See Also
- [Top-level Element: &lt;subject&gt;](https://www.loc.gov/standards/mods/userguide/subject.html) for official MODS documentation from the Library of Congress
- [Library of Congress Subject Headings: Online Training](https://www.loc.gov/catworkshop/lcsh/index.html) for training modules that cover the use of subject headings developed by Library of Congress staff
- [Library of Congress Subject Headings Manual](https://www.loc.gov/aba/publications/FreeSHM/freeshm.html) for an index of subject heading manuals published by by Library of Congress staff
- [NYPL Archival Processing Manual: Subjects](https://docs.google.com/document/d/1AD5DpkyzCEeBaBoAtAy71qo4tyabB2yy28xkkXx-P4s/edit#heading=h.9q8h9ik6hap8) for corresponding guidelines developed by the Library's Archival Processing department
