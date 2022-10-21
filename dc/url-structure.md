---
layout: page
title: URL Structure
permalink: /dc/url-structure/
parent: Digital Collections
nav_order: 4
---

# URL Structure

For consistency and reliability, we suggest using the following URL structures with Universal Unique Identifiers (UUID) to link to entities in Digital Collections

## Collection URLs

<dl>

<dt>Preferred structure</dt>
<dd><tt>https://digitalcollections.nypl.org/collections/<span style="color: #dd2e2e;">collection UUID</span></tt></dd>

<dt>Example</dt>
<dd><tt><a href="https://digitalcollections.nypl.org/collections/28d304b0-c612-012f-cd39-58d385a7bc34">https://digitalcollections.nypl.org/collections/28d304b0-c612-012f-cd39-58d385a7bc34</a></tt></dd>

</dl>

1. On Digital Collections, find the UUID for the collection by clicking the **About** tab for a collection
    1. The UUID will be found at the bottom of the **Collection Data** sidebar under **Identifiers**
1. In the Metadata Management System, the UUID can be found immediately below the collection title on any tab for the collection

{: .note-title }
> Note
>
> By default, the Digital Collections browser URL bar displays a URL with an encoded version of the collection title in lieu of the UUID. The MSU does not recommend using this URL as it is less stable and links will break in the event a collection title is changed.

## Container URLs
These URLs are currently very unstable as they change when containers are reordered or new containers added

> Container URLs are built on collection URLs. When creating links to Digital Collections containers, please ensure the base collection URL utilizes the collection UUID (please see the Collections URLs note above) rather than the encoded collection title

### Containers within Collections
Preferred URL structure: https://digitalcollections.nypl.org/collections/[collection UUID]/?tab=navigation&roots=[container sequence number followed by a : (only appears after first container in a collection)][container UUID]
Example URL (first container in collection): 
Example URL (second container in collection): 
Note: For nested containers, the URL structure pattern following "?tab=navigation&roots=" is repeated for each container, separated by  "/" 
On Digital Collections, find the container UUID at the very end of the URL in the browser URL bar
If the container is nested, the UUIDs for the root container and all other parent containers will also be present in the URL
In MMS, the UUID can be found immediately below the container title on any tab for the container
Containers within Containers
Preferred URL structure (nested): https://digitalcollections.nypl.org/collections/[collection UUID]/?tab=navigation&roots=[container sequence number followed by a : (only appears after first container in a collection)][container UUID]/[container sequence number followed by a : (only appears after first sub-container in a container)][container UUID]
Example URL (nested, first subcontainer in root container):
Example URL (nested, second subcontainer in root container):

## Item URLs
Preferred URL structure: https://digitalcollections.nypl.org/items/[item UUID]
Example URL: https://digitalcollections.nypl.org/items/85ae0f00-c63e-012f-11aa-58d385a7bc34#/?uuid=5e66b3e8-cd03-d471-e040-e00a180654d7
On Digital Collections, find UUID for the item in the "Identifiers" section at the bottom of an item page
In MMS, the UUID can be found immediately below the item title on any tab for the item


## Capture URLs
- Preferred URL structure: https://digitalcollections.nypl.org/items/[capture UUID]
- Example URL: 
- On Digital Collections, the full capture URL—including the UUID for the capture—is populated as a permalink, which can be found to the right of the IMAGE ID field directly below the image viewer
- In MMS, the UUID can be found immediately below the capture name on an individual capture page or in the UUID column of the an item's capture inventory page