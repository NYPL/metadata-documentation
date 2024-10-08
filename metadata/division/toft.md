---
layout: page
title: Theatre on Tape and Film
permalink: /division/toft/
parent: By Division
grand_parent: MMS › Metadata
nav_exclude: true
---

# Theatre on Film and Tape Archive
{: .no_toc }

Provides guidelines for metadata describing material from the Theatre on Film and Tape Archive (TOFT) in the Metadata Management System (MMS)

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Guidelines

---

### Record Structure
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Record Types →](/metadata-documentation/metadata/record-type/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- All TOFT records should be located within the collection that corresponds to whether the material should be publicly accessible:
  - **Restricted**: [Theatre on Film and Tape Archive Production Videos: RESTRICTED 🔒](https://metadata.nypl.org/collection/72886)
  - **Unrestricted**: [Theatre on Film and Tape Archive Public Program Videos 🔒](https://metadata.nypl.org/collection/73210)

---

### Name
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/name/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- Delete **Name** elements for TOFT directors (`Hoffman, Patrick` and `Corwin, Betty L.`)
  - Ensure their names are instead included in a [**Note**](#note) element with the **Type**: **statement of responsibility**
- For the **Name** element for the Theatre on Film and Tape Archive:
  - Ensure **Free text** is formatted exactly as `New York Public Library for the Performing Arts, Billy Rose Theatre Division, Theatre on Film and Tape Archive` (without any periods)
  - Add the **Role**: **Producer**
- For **Name** elements in the source record with the relator **Video producer** or **Series producer**:
  - Add the **Role**: **Producer**
- For **Name** elements in the source record with a relator containing the word `designer` and no exact-match [MARC relator term](https://www.loc.gov/marc/relators/relaterm.html) is available (e.g. **Projection designer** or **Puppet designer**):
  - Add the **Role**: **Designer**
- For **Name** elements in the source record with a relator containing the phrase `stage manager` (e.g. **Stage manager** or **Production stage manager**):
  - Add the **Role**: **Production personnel**
- For any **Name** elements where the relator was not imported and is not a [MARC relator term](https://www.loc.gov/marc/relators/relaterm.html) (e.g. **Orchestrations** or **Musical supervision)**:
  - Add the **Role**: **Contributor**
  
---

### Note
{: .d-inline .v-align-middle .mr-2 }
[View MSU Documentation for Element →](/metadata-documentation/metadata/element/note/)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

- If removing a **Name** element for TOFT directors (`Hoffman, Patrick` and `Corwin, Betty L.`), ensure their names are instead included in a [**Note**](https://docs.google.com/document/d/1729J2drDizJ3juW-RH3KIewgNvKLBo85o6nn82pjPMA/edit#note) element with the **Type**: **statement of responsibility**
  - The format of their names within the **statement of responsibility** should follow:
    - `Theatre on Film and Tape Archive, Patrick Hoffman, director`
    - `Theatre on Film and Tape Archive, Betty L. Corwin, director`

---

## See Also

- [Theatre on Film and Tape Archive (Internal Documentation) 🔒](https://docs.google.com/document/d/1ukxv__9sH0-CkDDYB3zkmp3_xkTl4O1Ae5qk5YSQ_3Y/edit) for the respective [MSU Liason's 🔒](https://docs.google.com/spreadsheets/d/1P-YDJigon640fTCLP4Ig4-zmzqrX88v5M24ShuxFNVY/edit?gid=0) internal documentation and notes related to the Theatre on Film and Tape Archive
- [MMS › Metadata › By Material › Audio and Moving Image (AMI)](/metadata-documentation/metadata/material/ami/) for guidelines for metadata specific to audio and moving image materials described in MMS