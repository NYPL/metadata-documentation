---
layout: page
title: Audio & Moving Image (AMI)
permalink: /metadata/material/ami/
parent: By Material
grand_parent: MMS › Metadata
nav_exclude: true
---

# Audio & Moving Image (AMI)
{: .no_toc }

Provides guidelines for metadata specific to audio and moving image (AMI) materials described in the Metadata Management System (MMS)

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Guidelines

---

### Identifier
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/identifier/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- Add AMI-related identifiers where applicable:
  - [AMI Identifier](/metadata-documentation/metadata/element/identifier/ami/)
  - [AMI Other ID](/metadata-documentation/metadata/element/identifier/ami-other/)
  - [AMI Primary Identifier](/metadata-documentation/metadata/element/identifier/ami-primary/)
  - [AMI Project](/metadata-documentation/metadata/element/identifier/ami-project/)
  - [Barcode](/metadata-documentation/metadata/element/identifier/barcode/)
  - [Capture Original Filename](/metadata-documentation/metadata/element/identifier/capture-original-filename/)
  - [CMS Collection Identifier](/metadata-documentation/metadata/element/identifier/cms-collection/)
  - [CMS Identifier](/metadata-documentation/metadata/element/identifier/cms/)

---

### Type of Resource
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/type-of-resource/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- Use **sound recording** for all audio
- Use **moving image** for all moving image

---

### Name
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/name/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- If the source MARC record contains an added entry for the title of the work ([NameTitle](https://id.loc.gov/ontologies/madsrdf/v1.html#NameTitle)) depicted in the recording, ensure the name component is added as a **Name** element with the appropriate [**Role**](/metadata-documentation/metadata/element/name/#role)
  - A [NameTitle](https://id.loc.gov/ontologies/madsrdf/v1.html#NameTitle) can be identified by the presence of 2 as an indicator in a [MARC 700](https://www.oclc.org/bibformats/en/7xx/700.html#:~:text=1946%2D%20%C7%82e%20actor-,2,%C7%82i%20Container%20of%20\(work\)%3A%20%C7%82a%20Aeschylus.%20%C7%82t%20Agamemnon,-Subfields) or [MARC 730](https://www.oclc.org/bibformats/en/7xx/730.html#:~:text=Code%20of%20Hammurabi-,2,%C7%82i%20Container%20of%20\(work\)%3A%20%C7%82a%20%27Twas%20the%20night%20before%20Christmas,-Subfields) field
  - E.g. [`Lloyd Webber, Andrew, 1948-`](https://legacycatalog.nypl.org/record=b16349574#:~:text=Lloyd%20Webber%2C%20Andrew%2C%201948%2D) is a **Name** element in the [item record](https://metadata.nypl.org/items/6051854?section=desc_md#:~:text=Lloyd%20Webber%2C%20Andrew%2C%201948%2D%20\(Composer\)) with the [**Role**](/metadata-documentation/metadata/element/name/#role) `composer`
- Do not indicate any **Name** element as [**Primary**](/metadata-documentation/metadata/element/name/#primary) for collaborative works
  - See the exception for moving image works in the relevant [content standard](/metadata-documentation/metadata/guidelines/#content-standards) for bibliographic materials, [RDA 6.27.1.3](https://original.rdatoolkit.org/lcpschp6_lcps6-348.html)

---

### Genre
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/genre/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- Add **Genre** based on the [Genre (AMI) 🔒](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1476737555) tab of the [Genre + Form + Extent 🔒](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit) spreadsheet

---

### Language
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/language/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- **Language** is required for AMI with linguistic content

---

### Physical Description
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/physical-description/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

---

#### Form
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Subelement →](/metadata-documentation/metadata/element/physical-description/#form)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- Add **Form** based on the [Form (AMI) 🔒](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1344175434) tab of the [Genre + Form + Extent 🔒](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit) spreadsheet

---

#### Extent
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Subelement →](/metadata-documentation/metadata/element/physical-description/#extent)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- Use **Extent** to describe the transfer master
  - For analog media, the transfer master is the analog format that was digitized
    - In some cases, this may be the archival original
    - In other cases, the archival original may have been transferred to another analog format that was subsequently digitized
  - For born-digital media, the transfer master is the archival original
  - For examples, see the [Extent Examples (AMI) 🔒](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=357146420) tab of the [Genre + Form + Extent 🔒](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit) spreadsheet

---

### Subject
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/subject/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

---

#### Title
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Subelement →](/metadata-documentation/metadata/element/subject/#title)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- If the source MARC record contains an added entry for the title of the work ([**NameTitle**](https://id.loc.gov/ontologies/madsrdf/v1.html#NameTitle)) depicted in the recording, ensure it is added as a **Title** subelement of **Subject**
  - A [NameTitle](https://id.loc.gov/ontologies/madsrdf/v1.html#NameTitle) can be identified by the presence of 2 as an indicator in a [MARC 700](https://www.oclc.org/bibformats/en/7xx/700.html#:~:text=1946%2D%20%C7%82e%20actor-,2,%C7%82i%20Container%20of%20\(work\)%3A%20%C7%82a%20Aeschylus.%20%C7%82t%20Agamemnon,-Subfields) or [MARC 730](https://www.oclc.org/bibformats/en/7xx/730.html#:~:text=Code%20of%20Hammurabi-,2,%C7%82i%20Container%20of%20\(work\)%3A%20%C7%82a%20%27Twas%20the%20night%20before%20Christmas,-Subfields) field
  - E.g. [`Lloyd Webber, Andrew, 1948- Joseph and the amazing Technicolor dreamcoat (Opera)`](https://legacycatalog.nypl.org/record=b16349574#:~:text=Lloyd%20Webber%2C%20Andrew%2C%201948%2D%20Joseph%20and%20the%20amazing%20Technicolor%20dreamcoat%20\(Opera\)) is a **Title** **Subject** in the [item record](https://metadata.nypl.org/items/6051854?section=desc_md#:~:text=Subject-,Lloyd%20Webber%2C%20Andrew%2C%201948%2D%20Joseph%20and%20the%20amazing%20Technicolor%20dreamcoat%20\(Opera\),-\(TitleInfo\))

---

## See Also

- [Audio and Moving Image (AMI)](/metadata-documentation/workflows/digitization/ami/) for guidelines pertaining to the ingest of AMI into MMS
- [AMI Metadata Overview](https://nypl.github.io/ami-preservation/pages/ami-metadata.html) for documentation of metadata requirements and controlled vocabulary from the Library’s Media Preservation units