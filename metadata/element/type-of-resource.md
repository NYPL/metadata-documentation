---
layout: page
title: Type of Resource
permalink: /metadata/element/type-of-resource/
parent: By Element
grand_parent: MMS › Metadata
nav_exclude: true
nav_order: 4
---

# Type of Resource
{: .d-inline .v-align-middle .no_toc .mr-2 }
Required
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
Repeatable
{: .d-inline .v-align-middle .label .label-green .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/typeofresource.html)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

A term that specifies the characteristics and general type of content of the resource
{: .d-block .mt-2 .fs-6 .fw-300 }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Purpose
- To support faceting of search results by general type and to help applications determine the appropriate viewing or playback system
- Categorizes the material in a general way
- More specific categorization is done in the [Genre](/metadata-documentation/metadata/element/genre/) element

## Guidelines
- Represents type of resource that applies to the content of the original resource, not the format of the digital surrogate
- For resources that include a combination of two or more types, this element is repeatable
    - Enter each applicable type in a new **Type of Resource** element
    - Mark one **Type of Resource** element as Primary

## Subelements

---

### Type of Resource
{: .d-inline .v-align-middle .mr-2 }
Required
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/typeofresource.html)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_A term that specifies the characteristics and general type of content of the resource_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Select the appropriate **Type of Resource** from the dropdown

<dl>

  <dt>text</dt>
  <dd>Resources that are basically textual in nature</dd>

  <dt>cartographic</dt>
  <dd>Includes maps, atlases, globes, digital maps, and other cartographic items</dd>

  <dt>notated music</dt>
  <dd>Graphic, non-realized representations of musical works, both in printed and digitized manifestations that represent the four components of musical sound: pitch, duration, timbre, and loudness</dd>

  <dt>sound recording</dt>
  <dd>Used when a mixture of musical and nonmusical sound recordings occurs in a resource or when a user does not want to or cannot make a distinction between musical and nonmusical</dd>

  <dt>still image</dt>
  <dd>Includes two-dimensional images and slides and transparencies</dd>

  <dt>moving image</dt>
  <dd>Includes motion pictures and videorecordings, as well as television programs, digital video, and animated computer graphics—but not slides and transparencies</dd>

  <dt>three dimensional object</dt>
  <dd>Includes man-made objects such as models, sculptures, clothing, and toys, as well as naturally occurring objects such as specimens mounted for viewing</dd>

  <dt>software, multimedia</dt>
  <dd>Appropriate for any electronic resource without a significant aspect that indicates one of the other categories</dd>

</dl>

Source: [Archived version of Top-level Element: &lt;typeOfResource&gt; (June 11, 2020)](https://web.archive.org/web/20200611002247/https://www.loc.gov/standards/mods/userguide/typeofresource.html)
{: .fs-2 }

- Use **sound recording** for all audio resources
    - Do not use **sound recording-musical** or **sound recording-nonmusical**

---

## Attributes

---

###  Primary
{: .d-inline .v-align-middle .mr-2 }
Required if Applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/attributes.html#usage)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_Used for a repeated element to declare that a particular instance of the element is most important_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Check **Primary** for <u>one</u> **Type of Resource** element if more than one **Type of Resource** element exists for a record

---

###  Manuscript
{: .d-inline .v-align-middle .mr-2 }
Do Not Use
{: .d-inline .v-align-middle .label .label-red .mx-1 }

#### Guidelines
{: .no_toc }
- This attribute is not in use at the present time, but legacy data may exist in MMS

---

### Collection
{: .d-inline .v-align-middle .mr-2 }
Do Not Use
{: .d-inline .v-align-middle .label .label-red .mx-1 }

#### Guidelines
{: .no_toc }
- This attribute is not in use at the present time, but legacy data may exist in MMS

---


## See Also
- [Top-level Element: &lt;typeOfResource&gt;](https://www.loc.gov/standards/mods/userguide/typeofresource.html) for official MODS documentation from the Library of Congress