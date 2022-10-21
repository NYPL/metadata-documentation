---
layout: page
title: URL Structure
permalink: /dc/url-structure/
parent: Digital Collections
nav_order: 3
---

# URL Structure
{: .no_toc }

For consistency and reliability when linking to entities in Digital Collections, we recommend using URLs structured according to the guidelines below

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Collection URLs

{: .note }
By default, the Digital Collections browser URL bar displays a URL with an encoded version of the collection title in lieu of the UUID. We do not recommend using this URL as it is less stable and links will break in the event a collection title is changed.

<dl>

<dt>Preferred structure</dt>
<dd><tt>https://digitalcollections.nypl.org/collections/<span style="background: #ffffcc; border: 1px solid #5c5962;">collection UUID</span></tt></dd>

<dt>Example</dt>
<dd><tt><a href="https://digitalcollections.nypl.org/collections/dba41b30-0ae6-0137-bfb0-4fa251ecd76a">https://digitalcollections.nypl.org/collections/<span style="background: #ffffcc; border: 1px solid #5c5962;">dba41b30-0ae6-0137-bfb0-4fa251ecd76a</span></a></tt></dd>

</dl>

### Finding UUIDs for Collections

- On <a href="https://digitalcollections.nypl.org">Digital Collections</a>, find the UUID by clicking the **About** tab for a collection
    - **Universal Unique Identifier (UUID)** will be found at the bottom of the **Collection Data** sidebar under **Identifiers**
- In the <a href="https://metadata.nypl.org">Metadata Management System</a>, the UUID can be found immediately below the collection's title following the **uuid:** label on any tab for the collection

## Container URLs

{: .warning }
Container URLs should be treated as less stable as they change when containers are reordered or new containers added.

{: .note }
Container URLs are built on their corresponding collection URLs. When creating links to Digital Collections containers, ensure the base collection URL utilizes the collection UUID (see <a href="#collection-urls">Collection URLs</a>) rather than the encoded collection title.

### Containers within Collections URLs

<dl>

<dt>Preferred structure</dt>
<dd><tt>https://digitalcollections.nypl.org/collections/<span style="background: #ffffcc; border: 1px solid #5c5962;">collection UUID</span>/?tab=navigation&roots=<span style="background: #cccccc; border: 1px solid #5c5962;">container sequence number followed by a : (only appears <em>after</em> first container in a collection)</span><span style="background: #ccffcc; border: 1px solid #5c5962;">container UUID</span></tt></dd>

<dt>Example<br>(1st container)</dt>
<dd><tt><a href="https://digitalcollections.nypl.org/collections/dba41b30-0ae6-0137-bfb0-4fa251ecd76a/?tab=navigation&roots=4c8bac10-0ae7-0137-4c89-5dcd471e46f5">https://digitalcollections.nypl.org/collections/<span style="background: #ffffcc; border: 1px solid #5c5962;">dba41b30-0ae6-0137-bfb0-4fa251ecd76a</span>/?tab=navigation&roots=<span style="background: #ccffcc; border: 1px solid #5c5962;">4c8bac10-0ae7-0137-4c89-5dcd471e46f5</span></a></tt></dd>

<dt>Example<br>(subsequent containers)</dt>
<dd><tt><a href="https://digitalcollections.nypl.org/collections/dba41b30-0ae6-0137-bfb0-4fa251ecd76a/?tab=navigation&roots=2:4d690980-0ae7-0137-49ea-3790db43fb92">https://digitalcollections.nypl.org/collections/dba41b30-0ae6-0137-bfb0-4fa251ecd76a/?tab=navigation&roots=<span style="background: #cccccc; border: 1px solid #5c5962;">2:</span><span style="background: #ccffcc; border: 1px solid #5c5962;">4d690980-0ae7-0137-49ea-3790db43fb92</span></a></tt></dd>

</dl>

### Containers within Containers URLs

{: .note }
For nested containers, the URL structure pattern following <tt>?tab=navigation&roots=</tt> is repeated for each container, separated by <tt>/</tt>.

<dl>

<dt>Preferred structure</dt>
<dd><tt>https://digitalcollections.nypl.org/collections/<span style="background: #ffffcc; border: 1px solid #5c5962;">collection UUID</span>/?tab=navigation&roots=<span style="background: #cccccc; border: 1px solid #5c5962;">1st container sequence number followed by a : (only appears <em>after</em> first container in a collection)</span><span style="background: #ccffcc; border: 1px solid #5c5962;">1st container UUID</span>/<span style="background: #999999; border: 1px solid #5c5962;">2nd container sequence number followed by a : (only appears <em>after</em> first container in a collection)</span><span style="background: #66cc66; border: 1px solid #5c5962;">2nd container UUID</span></tt></dd>

<dt>Example</dt>
<dd><a href="https://digitalcollections.nypl.org/collections/dba41b30-0ae6-0137-bfb0-4fa251ecd76a/?tab=navigation&roots=2:4d690980-0ae7-0137-49ea-3790db43fb92/2:7d05c7b0-c2ed-0139-8462-0242ac110003"><tt>https://digitalcollections.nypl.org/collections/<span style="background: #ffffcc; border: 1px solid #5c5962;">dba41b30-0ae6-0137-bfb0-4fa251ecd76a</span>/?tab=navigation&roots=<span style="background: #cccccc; border: 1px solid #5c5962;">2:</span><span style="background: #ccffcc; border: 1px solid #5c5962;">4d690980-0ae7-0137-49ea-3790db43fb92</span>/<span style="background: #999999; border: 1px solid #5c5962;">2:</span><span style="background: #66cc66; border: 1px solid #5c5962;">7d05c7b0-c2ed-0139-8462-0242ac110003</span></tt></a></dd>

</dl>

### Finding UUIDs for Containers

- On <a href="https://digitalcollections.nypl.org">Digital Collections</a>, find the UUID at the very end of the URL in the browser URL bar
    - If the container is nested, the UUIDs for the root container and all other parent containers will also be present in the URL
- In the <a href="https://metadata.nypl.org">Metadata Management System</a>, the UUID can be found immediately below the container's title following the **uuid:** label on any tab for the collection

## Item URLs

<dl>

<dt>Preferred structure</dt>
<dd><tt>https://digitalcollections.nypl.org/items/<span style="background: #ccccff; border: 1px solid #5c5962;">item UUID</span></tt></dd>

<dt>Example</dt>
<dd><tt><a href="https://digitalcollections.nypl.org/items/60d42da0-c2ee-0139-8909-0242ac110003">https://digitalcollections.nypl.org/items/<span style="background: #ccccff; border: 1px solid #5c5962;">60d42da0-c2ee-0139-8909-0242ac110003</span></a></tt></dd>

</dl>

### Finding UUIDs for Items

- On <a href="https://digitalcollections.nypl.org">Digital Collections</a>, find the UUID in the **Identifiers** section at the bottom of an item page
- In the <a href="https://metadata.nypl.org">Metadata Management System</a>, the UUID can be found immediately below the item's title following the **uuid:** label on any tab for the collection

## Capture URLs

<dl>

<dt>Preferred structure</dt>
<dd><tt>https://digitalcollections.nypl.org/items/<span style="background: #ffccff; border: 1px solid #5c5962;">capture UUID</span></tt></dd>

<dt>Example</dt>
<dd><tt><a href="https://digitalcollections.nypl.org/items/ce95c650-cafb-0139-aded-0242ac110002">https://digitalcollections.nypl.org/items/<span style="background: #ffccff; border: 1px solid #5c5962;">ce95c650-cafb-0139-aded-0242ac110002</span></a></tt></dd>

</dl>

### Finding UUIDs for Captures

- On <a href="https://digitalcollections.nypl.org">Digital Collections</a>, the full capture URL—including the UUID for the capture—is populated as the **Permalink**, which can be found to the right of the **Image ID** field directly below the image viewer
- In the <a href="https://metadata.nypl.org">Metadata Management System</a>, the UUID can be found immediately below the capture's title following the **uuid:** label on a capture page
    - Alternately, from a Capture Inventory page, capture UUIDs will be shown in the **UUID** column