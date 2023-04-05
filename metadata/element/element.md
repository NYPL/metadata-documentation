---
layout: page
title: By Element
permalink: /metadata/element/
parent: MMS › Metadata
nav_order: 3
has_children: true
has_toc: false
---

# By Element
These pages describe our local practices for each of the [Metadata Object Description Schema](/metadata-documentation/resources/glossary/#metadata-object-description-schema) (MODS) elements in the [Metadata Management System](/metadata-documentation/resources/glossary/#metadata-management-system) (MMS)

{: .note }
> In a typical workflow, metadata elements are populated automatically when [importing metadata](/metadata-documentation/workflows/import/) from other systems. These pages are intended as reference when reviewing the quality of imported metadata, [creating new metadata](/metadata-documentation/workflows/create/) from scratch, assessing whether [minimum metadata requirements](/metadata-documentation/metadata/guidelines/#minimum-metadata-requirements) are met, and/or aligning legacy records with local guidelines as part of [metadata remediation](/metadata-documentation/workflows/remediation/).

---

#### Elements
- [Title](/metadata-documentation/metadata/element/title/) <span class="label label-blue fs-1 mb-1 mx-1">Required</span>
- [Identifier](/metadata-documentation/metadata/element/identifier/) <span class="label label-blue fs-1 mb-1 mx-1">Required</span>
- [Type of Resource](/metadata-documentation/metadata/element/type-of-resource/) <span class="label label-blue fs-1 mb-1 mx-1">Required</span>
- [Origin Info](/metadata-documentation/metadata/element/origin-info/)
    - [Date](/metadata-documentation/metadata/element/origin-info/#date) <span class="label label-blue fs-1 mb-1 mx-1">Required</span>
- [Name](/metadata-documentation/metadata/element/name/)
- [Genre](/metadata-documentation/metadata/element/genre/) <span class="label label-blue fs-1 mb-1 mx-1">Required</span>
- [Language](/metadata-documentation/metadata/element/language/) <span class="label label-blue fs-1 mb-1 mx-1">Required if Applicable</span>
- [Physical Description](/metadata-documentation/metadata/element/physical-description/)
- [Subject](/metadata-documentation/metadata/element/subject/)
- [Abstract](/metadata-documentation/metadata/element/abstract/)
- [Table of Contents](/metadata-documentation/metadata/element/table-of-contents/)
- [Note](/metadata-documentation/metadata/element/note/)
- [Classification](/metadata-documentation/metadata/element/classification/)
- [Location](/metadata-documentation/metadata/element/location/) <span class="label label-blue fs-1 mb-1 mx-1">Required</span>

#### Guidelines

- <span class="label label-blue fs-1 mb-1 mx-1">Required</span> fields must exist at the item level, see [Minimum Metadata Requirements](/metadata-documentation/metadata/guidelines/#minimum-metadata-requirements)
 - <span class="label label-blue fs-1 mb-1 mx-1">Required if Applicable</span> fields are required if warranted by the specific resource being described
- <span class="label label-blue fs-1 mb-1 mx-1">Recommended</span> fields are optional but strongly recommended to be included if the information is readily available and if time and resources allow
- <span class="label label-blue fs-1 mb-1 mx-1">Recommended if Applicable</span> fields are recommended if certain constraints are met or if the information is available
- Fields marked as <span class="label label-red fs-1 mb-1 mx-1">Do Not Use</span> are not in use at the present time, but legacy data may exist in MMS

All other fields are optional and may be included at the metadata creator's discretion based on time and resources available

<!--
Template

# Element
{: .d-inline .v-align-middle .no_toc .mr-2 }
Required
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
Repeatable
{: .d-inline .v-align-middle .label .label-green .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/generalapp.html)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

Definition from MODS
{: .d-block .mt-2 .fs-6 .fw-300 }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Purpose
Lorem ipsem

## Guidelines
- Lorem ipsem

## Workflows

### Lorem ipsem

Lorem ipsem

## Subelements

---

### Subelement name
{: .d-inline .v-align-middle .mr-2 }
Required
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/generalapp.html)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_Definition from MODS_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Lorem ipsem

---

## Attributes

---

### Attribute name
{: .d-inline .v-align-middle .mr-2 }
Required
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/generalapp.html)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_Definition from MODS_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Lorem ipsem

---

## See Also
- [Top-level Element: &lt;TK&gt;](https://www.loc.gov/standards/mods/userguide/generalapp.html) for official MODS documentation from the Library of Congress

-->
