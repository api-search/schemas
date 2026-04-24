---
description: ''
layout: schema
name: Transaction
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: status
  type: string
- description: Raw transaction description from bank
  name: description
  type: string
- description: ''
  name: amount
  type: number
- description: ''
  name: balance
  type: number
- description: ''
  name: direction
  type: string
- description: Basiq transaction class (e.g., payment, transfer)
  name: class
  type: string
- description: ''
  name: subClass
  type: object
- description: ''
  name: transactionDate
  type: string
- description: ''
  name: postDate
  type: string
provider_name: Basiq
provider_slug: basiq
schema_file: json-schema/transaction.json
slug: transaction
tags:
- Australia
- Banking
- CDR
- Financial Data
- Fintech
- Open Banking
- Transactions
title: Transaction
---
