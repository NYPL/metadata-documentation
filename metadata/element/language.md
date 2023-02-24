---
layout: page
title: Language
permalink: /metadata/element/language/
parent: By Element
grand_parent: MMS › Metadata
nav_exclude: true
nav_order: 9
---

# Language
{: .d-inline .v-align-middle .no_toc .mr-2 }
Required if Applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
Repeatable
{: .d-inline .v-align-middle .label .label-green .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/language.html)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

The language in which the content of a resource is expressed
{: .d-block .mt-2 .fs-6 .fw-300 }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Purpose
- To indicate the language of a resource when textual or verbal content is present
- When consistently applied, this element can allow users to filter [Digital Collections](/metadata-documentation/resources/glossary/#digital-collections) search results by language

## Guidelines
- The **Language** element is required when language is primary to understanding the resource (i.e., if [**Type of Resource**](/metadata-documentation/metadata/element/type-of-resource/) is set to **text**, or if it is set to **sound recording** or **moving image** and verbal content is present)
    - This requirement includes when the resource is in English
- For resources where textual content is not the primary focus, such as image captions or sheet music lyrics, including the language of this content is optional but highly recommended
- For resources that contain multiple languages, this element is repeatable
    - Enter each applicable language in a new **Language** element
    - Mark one Language element as [**Primary**](#primary)

## Subelements

---

### Language
{: .d-inline .v-align-middle .mr-2 }
Required if Applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/language.html#languageterm)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_Contains the textual or coded form for the language of the content of the resource_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Select the appropriate **Language** from the dropdown
    - Values are based on [ISO 639.2](https://www.loc.gov/standards/iso639-2/php/code_list.php)
- If the **Language** cannot be determined, but is required due to presence of textual or verbal content, select **Undetermined**
- If there is no textual or verbal content, the **Language** element is not required

---

### Script
{: .d-inline .v-align-middle .mr-2 }
Recommended if Applicable
{: .d-inline .v-align-middle .label .label-blue .mx-1 }
[View MODS Documentation →](https://www.loc.gov/standards/mods/userguide/language.html#scriptterm)
{: .d-inline .v-align-middle .text-zeta .ml-2 }

_Contains the script(s) of the resource_
{: .d-block .mt-2 }

#### Guidelines
{: .no_toc }
- Script is recommended when the script of the title is not the default script of the language
- Select the appropriate **Script** from the dropdown
    - Values are based on [ISO 15924](https://www.iso.org/standard/29546.html)

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
- Check **Primary** for <u>one</u> **Language** element if more than one **Language** element exists for a record

---

## See Also
- [Top-level Element: &lt;language&gt;](https://www.loc.gov/standards/mods/userguide/language.html) for official MODS documentation from the Library of Congress