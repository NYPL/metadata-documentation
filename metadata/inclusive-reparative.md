---
layout: page
title: Inclusive & Reparative Description
permalink: /metadata/inclusive-reparative/
parent: MMS › Metadata
nav_order: 3
---

<style>code { white-space : pre-wrap !important; word-break: break-word; }</style>

# Inclusive & Reparative Description
{: .no_toc }

Provides context and workflows that support inclusive and reparative description in the context of the Metadata Management System (MMS)

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Overview
- Recognizing that libraries are not neutral, the Metadata Services Unit (MSU) has prioritized two parallel efforts:
  - [Inclusive description](#inclusive-description): the intentional creation of new metadata grounded in best practices developed to minimize bias and harm
  - [Reparative description](#reparative-description): the remediation of existing metadata that is harmful, biased, offensive, outdated, or inaccurate
- In addition to the general workflows and best practices described below, the MSU leads and participates in several [Projects](/metadata-documentation/projects/) related to inclusive and reparative description

## Reparative Description

### Steps for Non-MSU Staff
- The Metadata Service Unit (MSU) has a policy that all metadata in NYPL Digital Collections (DC) and Metadata Management System (MMS) is consistent with any corresponding description that exists in other Library systems
   - If harmful description or content found in DC/MMS also exists in other Library systems (e.g. catalog records, finding aids, or TMS records), MSU will work with you to ensure updates are made in those other systems first
   - If a source record has already been updated in another Library system that corresponds to digitized material in DC/MMS, let us know via our [contact form](/metadata-documentation/contact/form/)

#### Initiating Reparative Description Process
{: .d-inline .v-align-middle .mr-2 }
For Non-MSU Staff
{: .d-inline .v-align-middle .label .label-purple .mx-1 }
1. Use the [contact form](/metadata-documentation/contact/form/) to notify the MSU when you encounter either of the following in NYPL Digital Collections (DC) or its backend, Metadata Management System (MMS):
   1. Language used to describe materials that is harmful, biased, offensive, outdated, or inaccurate ("description")
   1. Resources that depict harmful or graphic content ("content")
1. Your submission will be reviewed by the [MSU liaison](/metadata-documentation/contact/#our-team) for the Library division or collection that holds the resource
   1. The liaison will review your submission to evaluate:
      - Whether your submission relates to description or content
      - If it is related to description, whether the description was created by Library staff or was transcribed directly (e.g. a title or caption written by the resource's creator that is visible in the digitized content)
      - If the description was created by Library staff, whether that description exists exclusively in DC/MMS or was imported from another source such as a MARC record or finding aid
   1. The liaison will implement the appropriate [workflows](#workflows)
   1. The liaison may also reach out to division staff to discuss any additional actions that may needed to address the reported issue such as:
      - Updating any source record(s)
      - Adding additional contextual notes, especially when subject expertise is needed
      - Suppressing content

### Steps for MSU Staff
- For workflows related to language used to describe material that is harmful, biased, offensive, outdated, or inaccurate ("description"), determine which of the following workflows is applicable:
  - If you wish to address description transcribed directly from the resource (e.g a title or caption written by the resource's creator that is visible in the digitized content), see [Addressing Description in Transcribed Elements](#addressing-description-in-transcribed-elements)
  - If you wish to address description created by Library staff, see [Addressing Description Created by Library Staff](#addressing-description-created-by-library-staff)
- For the workflow related to resources that depict harmful or graphic content ("content"), see [Addressing Harmful Content](#addressing-harmful-content)
- For workflows related to the intentional creation of new metadata grounded in best practices developed to minimize bias and harm, see [Inclusive Metadata](#inclusive-metadata)

#### Addressing Description in Transcribed Elements
{: .d-inline .v-align-middle .mr-2 }
For MSU Staff
{: .d-inline .v-align-middle .label .label-purple .mx-1 }
- Determine which [metadata element](/metadata-documentation/metadata/element/) contains the transcribed harmful, biased, offensive, outdated, or inaccurate description and follow the corresponding steps
  - [Title](#addressing-transcribed-title-elements)
  - [Non-Title Elements](#addressing-transcribed-non-title-elements) (e.g., Abstract or Note)

##### Addressing Transcribed Title Elements
{: .d-inline .v-align-middle .mr-2 }
For MSU Staff
{: .d-inline .v-align-middle .label .label-purple .mx-1 }
1. Add a new **Title** element that addresses the issues in the original **Title** element based on the relevant [guidelines](/metadata-documentation/metadata/element/title/#guidelines)
   1. Check **Primary**
   1. If [supplying](/metadata-documentation/metadata/element/title/#supplied) an entirely new title element, check **Supplied**
   1. If addressing only a specific portion of the text, enclose the corrected text in brackets, e.g. "[their]" to replace "thier" and do not check **Supplied**
1. In the original **Title** element:
   1. Uncheck **Primary**
   1. In the **Part Name** box, enter the source of the original title in square brackets (e.g. "`[caption title]`")
1. If further clarification is needed about the original or updated title, add a [**Note**](/metadata-documentation/metadata/element/note/)
   1. For the note **Type**, select **content**

{: .note-title }
> Example
>
> The official caption of a photograph incorrectly identified the people in the photograph:
> [https://metadata.nypl.org/items/4951434?section=desc_md 🔒](https://metadata.nypl.org/items/4951434?section=desc_md)

{: .note-title }
> Example
>
> The division wished to add a more descriptive title than what appeared on the image:
> [https://metadata.nypl.org/items/6232674?section=desc_md 🔒](https://metadata.nypl.org/items/6232674?section=desc_md)

##### Addressing Transcribed Non-Title Elements
{: .d-inline .v-align-middle .mr-2 }
For MSU Staff
{: .d-inline .v-align-middle .label .label-purple .mx-1 }
1. Ensure the transcribed description is clearly contextualized and attributed
1. [Add a harmful description note](#adding-a-harmful-description-note)

#### Addressing Description Created by Library Staff
{: .d-inline .v-align-middle .mr-2 }
For MSU Staff
{: .d-inline .v-align-middle .label .label-purple .mx-1 }
1. Determine which of the following criteria applies and follow the corresponding steps:
   1. Description was created by Library staff and matches description from the finding aid:
      1. For [divisions served by Archival Processing](https://docs.google.com/document/d/1tiIm0R8P0A_sOH3RUKsPgUKXAThqXT074QeIEokD6uk/edit#heading=h.gh2654hr28xp), work with Archival Processing to update the source finding aid using their [Archival Processing Unit Description Remediation Request](https://docs.google.com/forms/d/e/1FAIpQLSexaz5kCcCdw99U67Z7sVCgemlXpofl9HuegMmGYxcN8zBGCA/viewform) form
      1. For divisions _not_ served by Archival Processing, discuss with the [Manager, Metadata Services](/metadata-documentation/contact/) as the relevant contact can vary by division
      1. If the source finding aid _will not_ be updated, [add a harmful description note](#adding-a-harmful-description-note) instead
   1. Description was created by Library staff and matches description from the MARC record:
      1. Work with [division staff 🔒](https://docs.google.com/spreadsheets/d/1P-YDJigon640fTCLP4Ig4-zmzqrX88v5M24ShuxFNVY/edit) to update the source MARC record
         1. If necessary, submit a ticket via ServiceNow ([BookOps › Cataloging 🔒](https://nyplprod.service-now.com/nyplsp?id=sc_cat_item&sys_id=37d54594c4504d00f254019b5f40e91f&sysparm_category=2c3832e1139ee740c82e7e276144b022)) with the **Inquiry type**: **Sierra bib record error** indicating who in the division is the point person for the request
         1. When the source MARC record is updated, [revise the metadata](#revising-harmful-description) in MMS to match
      1. If the source MARC record _will not_ be updated, [add a harmful description note](#adding-a-harmful-description-note) instead
   1. Description was created by Library staff and matches description from a TMS record:
      1. Work with [division staff](https://docs.google.com/spreadsheets/d/1P-YDJigon640fTCLP4Ig4-zmzqrX88v5M24ShuxFNVY/edit) to determine how to update the source TMS record
         1. When the source TMS record is updated, [revise the metadata](#revising-harmful-description) in MMS to match
      1. If the source TMS record _will not_ be updated, [add a harmful description note](#adding-a-harmful-description-note) instead
   1. Description exists exclusively in MMS/DC:
      1. Work with [division staff](https://docs.google.com/spreadsheets/d/1P-YDJigon640fTCLP4Ig4-zmzqrX88v5M24ShuxFNVY/edit) to determine how to update the MMS/DC record
         1. [Revise the metadata](#revising-harmful-description)
      1. If the MMS/DC record _will not_ be updated, [add a harmful description note](#adding-a-harmful-description-note)

#### Adding a Harmful Description Note
{: .d-inline .v-align-middle .mr-2 }
For MSU Staff
{: .d-inline .v-align-middle .label .label-purple .mx-1 }
1. Add a new **Note** element by copying and pasting the following text:
```
This record may contain language that is harmful, inaccurate, or outdated. For more information, including information about how to contact us to report potentially harmful language, please refer to NYPL's Statement on Potentially Harmful Content for Digital Collections: https://digitalcollections.nypl.org/about#nypl_harmful_content_statement
```
   1. Add the above text without alteration as consistent usage will allow staff to locate harmful description records in the future
   1. If the above text does not seem applicable, discuss with the [Manager, Metadata Services](/metadata-documentation/contact/#our-team)
   1. For the note **Type**, select **content**

#### Revising Harmful Description
{: .d-inline .v-align-middle .mr-2 }
For MSU Staff
{: .d-inline .v-align-middle .label .label-purple .mx-1 }
1. Confirm you have met all the requirements necessary to revise metadata in MMS
   - Description was created by Library staff
   - Description is updated in the source record _or_ description exists exclusively in MMS/DC
   - [Creating Inclusive Description](#creating-inclusive-description) resources have been consulted
   - [Division staff 🔒](https://docs.google.com/spreadsheets/d/1P-YDJigon640fTCLP4Ig4-zmzqrX88v5M24ShuxFNVY/edit#gid=0\&range=F2:F37) have been consulted to determine new metadata
1. Update the metadata in MMS
   1. If the description should not be updated, [add a harmful description note](#adding-a-harmful-description-note)
1. If further clarification is needed about the original or updated metadata, add a [Note](/metadata-documentation/metadata/element/note/)
   1. For the note **Type**, select **content**

#### Addressing Harmful Content
{: .d-inline .v-align-middle .mr-2 }
For MSU Staff
{: .d-inline .v-align-middle .label .label-purple .mx-1 }
1. Consult with [division staff 🔒](https://docs.google.com/spreadsheets/d/1P-YDJigon640fTCLP4Ig4-zmzqrX88v5M24ShuxFNVY/edit#gid=0\&range=F2:F37) if you encounter harmful, difficult, or offensive content on MMS/DC or it is [reported](/metadata-documentation/workflows/remediation/feedback/) to you
   1. Division staff may request one or both of the following steps:
      1. The resource can be suppressed from public view in Digital Collections (resources cannot be deleted from MMS)
      1. A note can be added to the descriptive metadata
   1. If the Division requests suppression, follow the steps that correspond to the record type you want to [suppress](/metadata-documentation/workflows/remediation/suppressing/):
      1. [Collections](/metadata-documentation/workflows/remediation/suppressing/#suppressing-collections-for-harmful-content)
      1. [Containers](/metadata-documentation/workflows/remediation/suppressing/#suppressing-containers-for-harmful-content)
      1. [Items](/metadata-documentation/workflows/remediation/suppressing/#suppressing-items-for-harmful-content)
   1. If the Division requests a note:
      1. Add a new **Note** element by copying and pasting the following text:
      ```
      This record may contain content that is harmful or difficult to view. For more information, please refer to NYPL's Statement on Potentially Harmful Content for Digital Collections: https://digitalcollections.nypl.org/about#nypl_harmful_content_statement
      ```
1. Add the above text without alteration as consistent usage will allow staff to locate harmful content records in the future
   1. If the above text does not seem applicable, discuss with the [Manager, Metadata Services](/metadata-documentation/contact/#our-team)
1. For the note **Type**, select **content**

## Inclusive Description

### Describing People

1. If describing the race or ethnicity of any one individual person in [Title](/metadata-documentation/metadata/element/title/) or [Note](/metadata-documentation/metadata/element/note/), include the race or ethnicity for all people depicted in the resource
   1. Do not assume race, ethnicity, or gender of people; research how they self-identified where possible
   1. Use linguistically similar qualifiers in description, e.g. "black women" and "white women" or "African American women" and "Caucasian women"
   1. Do not describe only women as pretty or comment on their appearance, hair, or clothing while not describing men in a similar fashion

### External Resources for Inclusive Description

- [The DEI Metadata Handbook](https://iastate.pressbooks.pub/isudp-2024-153/)
- [Inclusive Metadata Toolkit](https://osf.io/2nmpc/)
- [Society of American Archivists Description Section › Inclusive Description](https://www2.archivists.org/groups/description-section/inclusive-description)
- [Yale University Reparative Archival Description Working Group](https://guides.library.yale.edu/c.php?g=1140330\&p=8319098)
- [Harvard University › Guidelines for Inclusive and Conscientious Description](https://wiki.harvard.edu/confluence/display/hmschommanual/Guidelines+for+Inclusive+and+Conscientious+Description)
- [Archives for Black Lives in Philadelphia Anti-Racist Description Resources](https://archivesforblacklives.files.wordpress.com/2020/11/ardr_202010.pdf#page=8)
- [Metadata Best Practices for Trans and Gender Diverse Resources](https://zenodo.org/doi/10.5281/zenodo.6686840)
- [Cataloging Lab](https://cataloginglab.org/)