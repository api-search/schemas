---
description: A dispensing, sealing, or packaging product from AptarGroup
layout: schema
name: Product
properties_list:
- description: Unique product identifier
  name: productId
  type: string
- description: Product name
  name: name
  type: string
- description: Product category (dispensing, sealing, active-packaging)
  name: category
  type: string
- description: Target market (beauty, pharma, food, home-care, etc.)
  name: market
  type: string
- description: Product description
  name: description
  type: string
- description: Primary material (plastic, aluminum, glass, etc.)
  name: material
  type: string
- description: Whether the product uses sustainable materials
  name: sustainable
  type: boolean
- description: Stock keeping unit identifier
  name: sku
  type: string
provider_name: AptarGroup
provider_slug: aptargroup
schema_file: json-schema/product-schema.json
slug: product
tags:
- Packaging
- Dispensing
- Manufacturing
- Sustainability
- Consumer Goods
title: Product
---
