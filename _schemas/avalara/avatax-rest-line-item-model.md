---
description: LineItemModel schema from Avalara API
layout: schema
name: LineItemModel
properties_list:
- description: Line number within the transaction
  name: number
  type: string
- description: Quantity of items
  name: quantity
  type: number
- description: Total amount for this line
  name: amount
  type: number
- description: Tax code for this line item
  name: taxCode
  type: string
- description: Item code for the product or service
  name: itemCode
  type: string
- description: Description of the line item
  name: description
  type: string
- description: ''
  name: addresses
  type: object
- description: Exemption code for tax-exempt purchases
  name: exemptionCode
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-line-item-model-schema.json
slug: avatax-rest-line-item-model
tags:
- Taxes
title: LineItemModel
---
