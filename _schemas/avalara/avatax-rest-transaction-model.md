---
description: TransactionModel schema from Avalara API
layout: schema
name: TransactionModel
properties_list:
- description: Unique ID of the transaction
  name: id
  type: integer
- description: Transaction code
  name: code
  type: string
- description: Company ID that owns this transaction
  name: companyId
  type: integer
- description: Date of the transaction
  name: date
  type: string
- description: Current status of the transaction
  name: status
  type: string
- description: Document type
  name: type
  type: string
- description: Total amount of the transaction before tax
  name: totalAmount
  type: number
- description: Total tax calculated for the transaction
  name: totalTax
  type: number
- description: Total taxable amount
  name: totalTaxable
  type: number
- description: Total exempt amount
  name: totalExempt
  type: number
- description: ''
  name: lines
  type: array
- description: ''
  name: addresses
  type: array
- description: ''
  name: summary
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-transaction-model-schema.json
slug: avatax-rest-transaction-model
tags:
- Taxes
title: TransactionModel
---
