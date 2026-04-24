---
description: JSON Schema for a Broadridge brokerage account transaction.
layout: schema
name: Broadridge Transaction
properties_list:
- description: ''
  name: transactionId
  type: string
- description: ''
  name: accountNumber
  type: string
- description: ''
  name: tradeDate
  type: string
- description: ''
  name: settleDate
  type: string
- description: ''
  name: transactionType
  type: string
- description: ''
  name: cusip
  type: string
- description: ''
  name: symbol
  type: string
- description: ''
  name: securityDescription
  type: string
- description: ''
  name: quantity
  type: number
- description: ''
  name: price
  type: number
- description: Net transaction amount after commissions and fees
  name: netAmount
  type: number
- description: Gross transaction amount before commissions and fees
  name: grossAmount
  type: number
- description: ''
  name: commission
  type: number
- description: ''
  name: fees
  type: number
- description: ''
  name: currency
  type: string
provider_name: broadridge
provider_slug: broadridge
schema_file: json-schema/broadridge-transaction-schema.json
slug: broadridge-transaction
tags: []
title: Broadridge Transaction
---
