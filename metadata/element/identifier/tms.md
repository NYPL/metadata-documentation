---
layout: page
title: TMS ID
permalink: /metadata/element/identifier/tms/
parent: Identifier
grand_parent: By Element
nav_exclude: true
---

# TMS ID
{: .d-inline .v-align-middle .no_toc .mr-2 }
Required if Applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }

Unique numeric identifier assigned to individual objects by the The Museum System (TMS), used by Print Collection and Photography Collection of the Miriam and Ira D. Wallach Division of Art, Prints and Photographs
{: .d-block .mt-2 .fs-6 .fw-300 }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Source
- ~~[The Museum System](/metadata-documentation/resources/glossary/#the-museum-system) (TMS)~~

## Guidelines
- ~~The **TMS ID** is automatically populated into records when [importing TMS records](/metadata-documentation/workflows/importing/tms/)~~
- ~~If adding a **TMS ID** to a record manually, it can be located in the [Prints & Photographs Online Catalog](https://wallachprintsandphotos.nypl.org/) as the numeric slug of the record's URL, e.g., [https://wallachprintsandphotos.nypl.org/catalog/**302742**](https://wallachprintsandphotos.nypl.org/catalog/302742)~~

{: .warning-title }
> Known Issue
>
> [TMS](/metadata-documentation/resources/glossary/#the-museum-system) and the [Prints & Photographs Online Catalog](/metadata-documentation/resources/glossary/#prints-photographs-online-catalog) were sunset in February 2024. While TMS records can no longer be imported, source data about items in the Print Collection and Photography Collection can manually copied from [Prints and Photographs Discovery](https://ppd.nypl.org/) (PPD) for now. **TMS ID**s can be found in PPD as the **object id**.
> <small><br>Last checked May 2025</small>

## Format

<dl>
<dt>Preferred structure</dt>
<dd><tt><span style="background: #ffccff; border: 1px solid #5c5962;">unique numeric identifier</span></tt></dd>
<dt>Example</dt>
<dd><a href="https://metadata.nypl.org/items/3371530?section=desc_md#:~:text=local_tms_id%3A-,302742,-Identifier"><tt><span style="background: #ffccff; border: 1px solid #5c5962;">302742</span></tt></a> (Print Collection)<br><a href="https://metadata.nypl.org/items/4310314?section=desc_md#:~:text=local_tms_id%3A-,8917,-Identifier"><tt><span style="background: #ffccff; border: 1px solid #5c5962;">8917</span></tt></a> (Photography Collection)</dd>

</dl>

## Inheritance
- **TMS ID** is typically assigned at the item level and not set to be inheritable
    - In rare cases where **TMS ID** is added to collections and containers, consider whether **TMS ID** should be **Inheritable** on a case-by-case basis

## Use With
- [TMS Object Number](/metadata-documentation/metadata/element/identifier/tms-object-number/#tms-object-number), the local classmark that corresponds to the **TMS ID**

## See Also
- [Prints and Photographs Discovery](https://ppd.nypl.org/) for source data about items in the Print Collection
- [The Museum System](/metadata-documentation/resources/glossary/#the-museum-system) for a corresponding definition in our glossary
- [Importing TMS Records](/metadata-documentation/workflows/importing/tms/) for a step-by-step of the process of importing records from TMS into the Metadata Management System (MMS)