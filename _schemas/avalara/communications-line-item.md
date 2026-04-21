---
description: LineItem schema from Avalara API
layout: schema
name: LineItem
properties_list:
- description: Line item reference
  name: ref
  type: string
- description: ''
  name: from
  type: object
- description: ''
  name: to
  type: object
- description: Charge amount
  name: chg
  type: number
- description: Number of lines
  name: line
  type: integer
- description: Number of locations
  name: loc
  type: integer
- description: Minutes
  name: min
  type: number
- description: Sale type (0=Wholesale, 1=Retail, 2=Consumed)
  name: sale
  type: integer
- description: Transaction type
  name: tran
  type: integer
- description: Service type
  name: serv
  type: integer
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/communications-line-item-schema.json
slug: communications-line-item
tags:
- Taxes
title: LineItem
---
