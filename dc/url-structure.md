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

{: .note-title }
> Major Update
>
> The structure of Digital Collections URLs changed with the redesign of Digital Collections in 2025. If you are looking for documentation of how URL structure worked prior to summer 2025, view an <a href="https://web.archive.org/web/20250806203243/https://nypl.github.io/metadata-documentation/dc/url-structure/">archived version of this page</a>.
> <small><br>August 2025</small>

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Collection URLs

<dl>

<dt>Preferred structure</dt>
<dd><tt>https://digitalcollections.nypl.org/collections/<span style="background: #ffffcc; border: 1px solid #5c5962;">collection UUID</span></tt></dd>

<dt>Example</dt>
<dd><tt><a href="https://digitalcollections.nypl.org/collections/dba41b30-0ae6-0137-bfb0-4fa251ecd76a">https://digitalcollections.nypl.org/collections/<span style="background: #ffffcc; border: 1px solid #5c5962;">dba41b30-0ae6-0137-bfb0-4fa251ecd76a</span></a></tt></dd>

</dl>

### Finding Collection UUIDs

- On <a href="https://digitalcollections.nypl.org">Digital Collections</a>, find the collection UUID either:
    - By clicking **See more collection information** and looking in the **Identifiers** section as the **Universal Unique Identifier (UUID)**
    - In the browser URL bar at the end of the full collection URL
- In the <a href="https://metadata.nypl.org">Metadata Management System</a>, the collection UUID can be found immediately below the collection's title following the **uuid:** label on any tab for the collection

## Container URLs

{: .note }
Container URLs are built using the parent <a href="#collection-urls">collection URLs</a>. When creating links to Digital Collections containers, you will also need the <a href="#finding-collection-uuids">collection UUID</a>.

<dl>

<dt>Preferred structure</dt>
<dd><tt>https://digitalcollections.nypl.org/collections/<span style="background: #ffffcc; border: 1px solid #5c5962;">collection UUID</span>?filters=%5Bsubcollection%3D<span style="background: #ccffcc; border: 1px solid #5c5962;">container UUID</span>%5D</tt></dd>

<dt>Example<br></dt>
<dd><tt><a href="https://digitalcollections.nypl.org/collections/dba41b30-0ae6-0137-bfb0-4fa251ecd76a?filters=%5Bsubcollection%3D4d66d980-0ae7-0137-4d11-7bf3d182b328%5D">https://digitalcollections.nypl.org/collections/<span style="background: #ffffcc; border: 1px solid #5c5962;">dba41b30-0ae6-0137-bfb0-4fa251ecd76a</span>?filters=%5Bsubcollection%3D<span style="background: #ccffcc; border: 1px solid #5c5962;">4d66d980-0ae7-0137-4d11-7bf3d182b328</span>%5D</a></tt></dd>

</dl>

### Finding Container UUIDs

- On <a href="https://digitalcollections.nypl.org">Digital Collections</a>, find the container UUID in the browser URL bar at the end of the full container URL between `?filters=%5Bsubcollection%3D` and `%5D`
- In the <a href="https://metadata.nypl.org">Metadata Management System</a>, the container UUID can be found immediately below the container's title following the **uuid:** label on any tab for the container

## Item URLs

<dl>

<dt>Preferred structure</dt>
<dd><tt>https://digitalcollections.nypl.org/items/<span style="background: #ccccff; border: 1px solid #5c5962;">item UUID</span></tt></dd>

<dt>Example</dt>
<dd><tt><a href="https://digitalcollections.nypl.org/items/60d42da0-c2ee-0139-8909-0242ac110003">https://digitalcollections.nypl.org/items/<span style="background: #ccccff; border: 1px solid #5c5962;">60d42da0-c2ee-0139-8909-0242ac110003</span></a></tt></dd>

</dl>

### Finding Item UUIDs

- On <a href="https://digitalcollections.nypl.org">Digital Collections</a>, find the collection UUID either:
    - In the **Identifiers** section as the **Universal Unique Identifier (UUID)**
    - In the browser URL bar at the end of the item URL before the `?canvasIndex=`
- In the <a href="https://metadata.nypl.org">Metadata Management System</a>, the item UUID can be found immediately below the item's title following the **uuid:** label on any tab for the item

## Capture URLs

<dl>

<dt>Preferred structure</dt>
<dd><tt>https://digitalcollections.nypl.org/items/<span style="background: #ccccff; border: 1px solid #5c5962;">item UUID</span>?canvasIndex=<span style="background: #ffccff; border: 1px solid #5c5962;">capture sequence number</span></tt></dd>

<dt>Example</dt>
<dd><tt><a href="https://digitalcollections.nypl.org/items/60d42da0-c2ee-0139-8909-0242ac110003?canvasIndex=8">https://digitalcollections.nypl.org/items/<span style="background: #ccccff; border: 1px solid #5c5962;">60d42da0-c2ee-0139-8909-0242ac110003</span>?canvasIndex=<span style="background: #ffccff; border: 1px solid #5c5962;">8</span></a></tt></dd>

</dl>

### Finding Capture UUIDs

{: .note }
Capture UUIDs are not used for <a href="#capture-urls"> capture URLs</a>.

- In the <a href="https://metadata.nypl.org">Metadata Management System</a>, the capture UUID can be found in the capture record or **Capture Inventory** tab
    - From a capture record, the UUID can be found immediately below the capture's title following the **uuid:** label
    - From the **Capture Inventory** tab on an item record, capture UUIDs will be shown in the **UUID** column