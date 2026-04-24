---
description: A software product in the Vendr catalog with structured attributes, features, and add-ons
layout: schema
name: Product
properties_list:
- description: Unique product identifier
  name: id
  type: string
- description: Product name
  name: name
  type: string
- description: Associated vendor identifier
  name: vendor_id
  type: string
- description: Product category
  name: category
  type: string
- description: Product description
  name: description
  type: string
- description: List of product features
  name: features
  type: array
- description: Available product add-ons
  name: add_ons
  type: array
provider_name: Blissfully
provider_slug: blissfully
schema_file: json-schema/blissfully-product-schema.json
slug: blissfully-product
tags:
- Procurement
- SaaS Discovery
- SaaS Management
- Software Procurement
- Spend Optimization
- Vendor Management
title: Product
---
