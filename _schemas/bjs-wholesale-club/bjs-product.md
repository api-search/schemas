---
description: Schema for a BJ's Wholesale Club product record
layout: schema
name: BJS Product
properties_list:
- description: Unique product identifier
  name: productId
  type: string
- description: Product display name
  name: name
  type: string
- description: Full product description
  name: description
  type: string
- description: ''
  name: brand
  type: string
- description: ''
  name: category
  type: string
- description: ''
  name: subcategory
  type: string
- description: Member price in USD
  name: price
  type: number
- description: Regular retail price in USD
  name: regularPrice
  type: number
- description: Unit of measure
  name: unit
  type: string
- description: ''
  name: images
  type: array
- description: ''
  name: memberExclusive
  type: boolean
- description: ''
  name: inStock
  type: boolean
provider_name: BJ's Wholesale Club
provider_slug: bjs-wholesale-club
schema_file: json-schema/bjs-product-schema.json
slug: bjs-product
tags:
- Ecommerce
- Membership
- Retail
- Wholesale
title: BJS Product
---
