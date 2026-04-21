---
description: CreateTransactionModel schema from Avalara API
layout: schema
name: CreateTransactionModel
properties_list:
- description: The type of document to create
  name: type
  type: string
- description: Company code of the company creating this transaction
  name: companyCode
  type: string
- description: Date of the transaction
  name: date
  type: string
- description: Unique code identifying the customer
  name: customerCode
  type: string
- description: Whether to commit the transaction immediately
  name: commit
  type: boolean
- description: Three-character ISO 4217 currency code
  name: currencyCode
  type: string
- description: ''
  name: addresses
  type: object
- description: Line items for the transaction
  name: lines
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-create-transaction-model-schema.json
slug: avatax-rest-create-transaction-model
tags:
- Taxes
title: CreateTransactionModel
---
