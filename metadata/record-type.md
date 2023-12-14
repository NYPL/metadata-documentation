---
layout: page
title: By Record Type
permalink: /metadata/record-type/
parent: MMS › Metadata
nav_order: 5
---

# By Record Type
{: .no_toc }

The Metadata Management System (MMS) supports four types of records that contain descriptive content and provide organization for digitized material, each of which have their own properties and descriptive practices

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Record Types

### Collections
* Collections are the highest record in the hierarchy
* Collections can contain containers and/or items
* Collections generally mimic the organization of the physical collection
* Collection records are typically imported from a finding aid or catalog record
* Collection records may also be created in MMS where no source finding aid or catalog record exists, although this is less common

### Containers
* Containers are intermediary records
* Containers can contain other containers and/or items
* Containers must be contained by a collection
* A collection can have zero or an unlimited number of containers

### Items
* Items can be standalone or contained in collections
* Items in collections can be contained just by a collection and/or any of the collection's containers
* Collections and containers can contain an unlimited number of items

### Captures
* Captures are attached to item records
* Each capture can have a single corresponding image, video, or audio asset
* An item can have zero or an unlimited number of captures
* Capture records do not have [MODS elements](/metadata-documentation/metadata/element/) associated with other record types
* Besides system-generated fields, captures have two editable fields:
    * **Name**: typically the same as the image ID generated during digitization process, but can be manually edited if deemed necessary
    * **Relationship**: a drop-down menu of values that can provide detail about what the capture is or how it relates to the item

## Hierarchy Examples

### Standalone Item
```
| -- Item
```

### Collection with Only Items
```
| -- Collection
   | -- Item
   | -- Item
   | -- Item
```

### Collection with Only Containers That Have Items
```
| -- Collection
   | -- Container
      | -- Item
      | -- Item
   | -- Container
      | -- Item
      | -- Item
```

### Collection with Both Containers and Items
```
| -- Collection
   | -- Container
      | -- Item
      | -- Item
   | -- Container
      | -- Item
      | -- Item
   | -- Item
   | -- Item
```

## See Also
* [Inheritance](/metadata-documentation/metadata/guidelines/#inheritance) for an explanation of how metadata elements from Collections and Containers can be set to inherit down to contained Containers and/or Items
* [By Element](/metadata-documentation/metadata/element/) for field-specific metadata guidance, which may include guidelines for specific record types
* [Digital Collections API: A note about our data model](https://api.repo.nypl.org/#data-model) for an explanation of record types in relation to the application programming interface for Digital Collections
