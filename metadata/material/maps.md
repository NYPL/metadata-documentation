---
layout: page
title: Maps
permalink: /metadata/material/maps/
parent: By Material
grand_parent: MMS › Metadata
nav_exclude: true
---

# Maps
{: .no_toc }

Provides guidelines for metadata specific to maps (or records with `cartographic` as the [Type of Resource](/metadata-documentation/metadata/element/type-of-resource/)) described in the Metadata Management System (MMS)

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Guidelines

---

### Genre
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/genre/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- Add **Genre** based on the of the [Genre (non-AMI) 🔒](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit#gid=1262013027\&fvid=1933164069) tab of the [Genre + Form + Extent 🔒](https://docs.google.com/spreadsheets/d/1NGlV94Iufe0p3EJdoJDX7SgvH-LUYqWLEuB1Az3DmbM/edit) spreadsheet
    - The tab has been filtered to displays genre terms with the **cartographic** in the  **common/primary type of resource(s)** field

---

### Note
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/note/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- Combine and relocate any longform **Note** elements with descriptive content to the [**Abstract**](/metadata-documentation/metadata/element/abstract/) element
  - If there are only one or two notes that don't form a comprehensive description of the resource, they can remain as a **Note** and with the **Type**: **content**
- Add the source record's [MARC 590](https://www.oclc.org/bibformats/en/5xx/590.html) ("Local Note") to the appropriate element:
  - Add as a **Note** and set the **Type** to **content** if the local note does not relate to the physical characteristics of the resource
  - Alternately, relocate the note to a [**Note**](/metadata-documentation/metadata/element/physical-description/#note) subelement of [**Physical Description**](/metadata-documentation/metadata/element/physical-description/) if the local note relates to the physical characteristics of the resource
- The source record's [MARC 255](https://www.oclc.org/bibformats/en/2xx/255.html) including [$a](https://www.oclc.org/bibformats/en/2xx/255.html#subfielda) ("Statement of scale"), [$b](https://www.oclc.org/bibformats/en/2xx/255.html#subfieldb) ("Statement of projection"), and [$c](https://www.oclc.org/bibformats/en/2xx/255.html#subfieldc) ("Statement of coordinates") can remain as a **Note** with the **Type**: **content**
- The [current version of MODS](/metadata-documentation/metadata/guidelines/#metadata-schema) used by the Metadata Management System does not yet support [Subelement: &lt;place&gt;&lt;cartographics&gt;](https://www.loc.gov/standards/mods/userguide/origininfo.html#oiplacecartographics)

---

## See Also

- [Cataloger's Reference Shelf Map Cataloging Manual](https://www.itsmarc.com/crs/mergedprojects/mapcat/mapcat/special_treatment_format.htm) for detailed guidelines by category of map created by the Library of Congress
