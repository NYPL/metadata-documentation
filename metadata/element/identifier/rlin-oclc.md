---
layout: page
title: RLIN/OCLC
permalink: /metadata/element/identifier/rlin-oclc/
parent: Identifier
grand_parent: By Element
nav_exclude: true
---

# RLIN/OCLC
{: .d-inline .v-align-middle .no_toc .mr-2 }
Unique identifier assigned by OCLC for a bibliographic record in WorldCat
{: .d-block .mt-2 .fs-6 .fw-300 }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Source
- [OCLC](https://www.oclc.org/bibformats/en/fixedfield/oclc.html) bibliographic records

## Guidelines
- The **RLIN/OCLC** identifier is automatically populated into records when [importing MARC records](/metadata-documentation/workflows/create-import/#importing-marc-records) as long as it is present in the source record
- If adding a RLIN/OCLC identifier to a record manually, it can be found:
    - In the [Research Catalog](/metadata-documentation/resources/glossary/#research-catalog) in the **OCLC** field of the record
    - In the [Legacy Catalog](/metadata-documentation/resources/glossary/#legacy-catalog) by [viewing the record's MARC XML](/metadata-documentation/resources/tips-tricks/#view-marc-in-legacy-catalog)
        - Confirm that ``<MARCFIXDATA>OCoLC</MARCFIXDATA>`` is present for the ``<MARCTAG>003</MARCTAG>`` tag of the bibliographic record
        - Search for the ``<VARFLD>`` that contains ``<MARCTAG>001</MARCTAG>``
        - The **RLIN/OCLC** identifier is the value present within the ``<MARCFIXDATA></MARCFIXDATA>`` tag, e.g., the **RLIN/OCLC** identifier for [b14903434](https://legacycatalog.nypl.org/xrecord=b14903434) is ``29052368``

## Format

{: .note }
OCLC numbers have replaced RLIN (Research Libraries Information Network) identifiers over time. The format documented here applies specifically to OCLC numbers. Although RLIN (Research Libraries Information Network) identifiers have been deprecated, legacy data may exist in the Library's MARC records and in MMS.

<dl>
<dt>Preferred structure</dt>
<dd><tt><span style="background: #ffccff; border: 1px solid #5c5962;">unique numeric identifier</span></tt></dd>
<dt>Example</dt>
<dd><a href="https://metadata.nypl.org/items/6292815?section=desc_md#:~:text=RLIN/OCLC%3A-,1133653761,-Identifier"><tt><span style="background: #ffccff; border: 1px solid #5c5962;">1133653761</span></tt></a></dd>
</dl>

## Inheritance
- Do not set **RLIN/OCLC** identifiers added to collections or containers to be **Inheritable**

## Use With
- [NYPL catalog ID (B-number)](/metadata-documentation/metadata/element/identifier/bnumber/), which is the primary identifier for a bibliographic record in Sierra, where **RLIN/OCLC** identifiers are ingested from

## See Also
- [OCLC Control Number](https://www.oclc.org/bibformats/en/fixedfield/oclc.html) for corresponding documentation from OCLC Support & Training
- [MARC 0xx](https://www.oclc.org/bibformats/en/0xx.html) for corresponding documentation from OCLC Support & Training
- [MARC 001 - Control Number (NR)](https://www.loc.gov/marc/bibliographic/bd001.html) for corresponding documentation from the Library of Congress