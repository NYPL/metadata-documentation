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

This page provides context and workflows that support inclusive and reparative description in the context of the Metadata Management System (MMS)

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

### Workflows (For Non-MSU Staff)

{: .note }
The Metadata Service Unit (MSU) has a policy that all metadata in NYPL Digital Collections (DC) and Metadata Management System (MMS) is consistent with any corresponding description that exists in other Library systems. If harmful description or content found in DC/MMS also exists in other Library systems (i.e. catalog records, finding aids, or TMS records), MSU will work with you to ensure updates are made in those other systems first. If a source record has already been updated in another Library system that corresponds to digitized material in DC/MMS, let us know via our [contact form](/metadata-documentation/contact/form/).

1. Use the [contact form](/metadata-documentation/contact/form/) to notify the MSU when you encounter either of the following in NYPL Digital Collections (DC) or its backend, Metadata Management System (MMS):
   1. Language used to describe materials that is harmful, biased, offensive, outdated, or inaccurate ("description")
   1. Resources that depict harmful or graphic content ("content")
1. Your submission will be reviewed by the [MSU liaison](/metadata-documentation/contact/#our-team) for the Library division or collection that holds the resource
   1. The liaison will review your submission to evaluate:
      - Whether your submission relates to description or content
      - If it is related to description, whether the description was created by Library staff or was transcribed directly (e.g. a title or caption written by the resource’s creator that is visible in the digitized content)
      - If the description was created by Library staff, whether that description exists exclusively in DC/MMS or was imported from another source such as a MARC record or finding aid
   1. The liaison will implement the appropriate [workflows](#workflows-for-msu-staff)
   1. The liaison may also reach out to division staff to discuss any additional actions that may needed to address the reported issue such as:
      - Updating any source record(s)
      - Adding additional contextual notes, especially when subject expertise is needed
      - Suppressing content

### Workflows (For MSU Staff)

- For workflows related to language used to describe material that is harmful, biased, offensive, outdated, or inaccurate ("description"), determine which of the following workflows is applicable:
  - If you wish to address description transcribed directly from the resource (e.g a title or caption written by the resource’s creator that is visible in the digitized content), see [Addressing Description in Transcribed Elements](#addressing-description-in-transcribed-elements)
  - If you wish to address description created by Library staff, see [Addressing Description Created by Library Staff](#addressing-description-created-by-library-staff)
- For the workflow related to resources that depict harmful or graphic content ("content"), see [Addressing Harmful Content](#addressing-harmful-content)
- For workflows related to the intentional creation of new metadata grounded in best practices developed to minimize bias and harm, see [Inclusive Metadata](#inclusive-metadata)

#### Addressing Description in Transcribed Elements
- Determine which [metadata element](/metadata-documentation/metadata/element/) contains the transcribed harmful, biased, offensive, outdated, or inaccurate description and follow the corresponding steps
  - [Title](#addressing-transcribed-title-elements)
  - [Non-Title Elements](#addressing-transcribed-non-title-elements) (e.g., Abstract or Note)

##### Addressing Transcribed Title Elements

1. Add a new **Title** element that addresses the issues in the original **Title** element (see [Title element guidelines](/metadata-documentation/metadata/element/title/#guidelines))
   1. If correcting only a specific portion of the text, enclose the corrected text in brackets, e.g. "[their]" to replace "thier"
   1. Check **Primary** and **Supplied** for the new **Title** element
1. In the original **Title** element:
   1. Uncheck **Primary**
   1. In the **Part Name** box, enter the source of the original title in square brackets (i.e. "\[caption title]")
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

1. Ensure the transcribed description is clearly contextualized and attributed
1. [Add a harmful description note](#adding-a-harmful-description-note)

#### Addressing Description Created by Library Staff

1. Determine which of the following criteria applies and follow the corresponding steps:
   1. Description was created by Library staff and matches description from the finding aid, [add a harmful description note](#adding-a-harmful-description-note)
   1. Description was created by Library staff and matches description from the MARC record:
      1. Work with [division staff 🔒](https://docs.google.com/spreadsheets/d/1P-YDJigon640fTCLP4Ig4-zmzqrX88v5M24ShuxFNVY/edit) to update the source MARC record
         1. If necessary, submit a ticket via ServiceNow ([BookOps › Cataloging 🔒](https://nyplprod.service-now.com/nyplsp?id=sc_cat_item\&sys_id=37d54594c4504d00f254019b5f40e91f)) with the **Inquiry type**: **Sierra bib record error** indicating who in the division is the point person for the request
         1. When the source MARC record is updated, [revise the metadata](#revising-harmful-description) in MMS to match
      1. If the source MARC record _will not_ be updated, [add a harmful description note](#adding-a-harmful-description-note) instead
   1. Description was created by Library staff and matches description from a TMS record:
      1. Work with [division staff](https://docs.google.com/spreadsheets/d/1P-YDJigon640fTCLP4Ig4-zmzqrX88v5M24ShuxFNVY/edit) to determine how to update the source TMS record
         1. When the source TMS record is updated, [revise the metadata](#revising-harmful-description) in MMS to match
      1. If the source TMS record _will not_ be updated, [add a harmful description note](#adding-a-harmful-description-note) instead
   1. Description exists exclusively in MMS/DC,
      1. Work with [division staff](https://docs.google.com/spreadsheets/d/1P-YDJigon640fTCLP4Ig4-zmzqrX88v5M24ShuxFNVY/edit) to determine how to update the MMS/DC record
         1. [Revise the metadata](#revising-harmful-description)
      1. If the MMS/DC record _will not_ be updated, [add a harmful description note](#adding-a-harmful-description-note)

#### Adding a Harmful Description Note

1. Add a new **Note** element by copying and pasting the following text:
```
This record may contain language that is harmful, inaccurate, or outdated. For more information, including information about how to contact us to report potentially harmful language, please refer to NYPL's Statement on Potentially Harmful Content for Digital Collections: https://digitalcollections.nypl.org/about#nypl_harmful_content_statement
```
   1. Add the above text without alteration as consistent usage will allow staff to locate harmful description records in the future
   1. If the above text does not seem applicable, discuss with the [Manager, Metadata Services](/metadata-documentation/contact/#our-team)
   1. For the note **Type**, select **content**

#### Revising Harmful Description

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

1. Consult with [division staff 🔒](https://docs.google.com/spreadsheets/d/1P-YDJigon640fTCLP4Ig4-zmzqrX88v5M24ShuxFNVY/edit#gid=0\&range=F2:F37) if you encounter harmful, difficult, or offensive content on MMS/DC or it is [reported](/metadata-documentation/workflows/remediation/feedback/) to you
   1. Division staff may request one or both of the following steps:
      1. The resource can be suppressed from public view in Digital Collections (resources cannot be deleted from MMS)
      1. A note can be added to the descriptive metadata
   1. If the Division requests suppression:
      1. Navigate to the **Rights and use** tab of an item record
      1. Select **Suppress from website**
      1. Do not select a **Reason**
      1. Add an explanation in the **Notes** field of the suppression prompt, e.g. `division requested suppression for harmful content [add date]`
      1. Click the **Suppress record** button
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

- [Society of American Archivists Description Section › Inclusive Description](https://www2.archivists.org/groups/description-section/inclusive-description)
- [Yale University Reparative Archival Description Working Group](https://guides.library.yale.edu/c.php?g=1140330\&p=8319098)
- [Harvard University › Guidelines for Inclusive and Conscientious Description](https://wiki.harvard.edu/confluence/display/hmschommanual/Guidelines+for+Inclusive+and+Conscientious+Description)
- [Archives for Black Lives in Philadelphia Anti-Racist Description Resources](https://archivesforblacklives.files.wordpress.com/2020/11/ardr_202010.pdf#page=8)
- [Metadata Best Practices for Trans and Gender Diverse Resources](https://zenodo.org/doi/10.5281/zenodo.6686840)
- [Cataloging Lab](https://cataloginglab.org/)