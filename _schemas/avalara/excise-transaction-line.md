---
description: TransactionLine schema from Avalara API
layout: schema
name: TransactionLine
properties_list:
- description: ''
  name: lineNumber
  type: string
- description: Excise product code
  name: productCode
  type: string
- description: Unit of measure
  name: unitOfMeasure
  type: string
- description: Quantity of product
  name: quantity
  type: number
- description: Line amount
  name: amount
  type: number
- description: ''
  name: origin
  type: object
- description: ''
  name: destination
  type: object
- description: ''
  name: billOfLadingNumber
  type: string
- description: ''
  name: carrierName
  type: string
- description: ''
  name: modeOfTransport
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/excise-transaction-line-schema.json
slug: excise-transaction-line
tags:
- Taxes
title: TransactionLine
---
