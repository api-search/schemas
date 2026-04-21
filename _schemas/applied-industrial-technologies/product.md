---
description: An industrial product distributed by Applied Industrial Technologies
layout: schema
name: Product
properties_list:
- description: Unique product identifier
  name: productId
  type: string
- description: Manufacturer part number
  name: partNumber
  type: string
- description: Product name
  name: name
  type: string
- description: Product description
  name: description
  type: string
- description: Product category (bearings, power transmission, etc.)
  name: category
  type: string
- description: Product manufacturer
  name: manufacturer
  type: string
- description: Unit price in USD
  name: price
  type: number
- description: Whether the product is in stock
  name: inStock
  type: boolean
- description: Lead time in days if not in stock
  name: leadTimeDays
  type: integer
provider_name: Applied Industrial Technologies
provider_slug: applied-industrial-technologies
schema_file: json-schema/product-schema.json
slug: product
tags:
- Industrial Distribution
- Bearings
- Power Transmission
- Fluid Power
- Supply Chain
title: Product
---
