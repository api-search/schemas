---
description: Account balance record
layout: schema
name: Balance
properties_list:
- description: ''
  name: accountId
  type: string
- description: Balance type (current, available, intraday)
  name: balanceType
  type: string
- description: ''
  name: amount
  type: number
- description: ''
  name: currency
  type: string
- description: ''
  name: asOfDateTime
  type: string
- description: ''
  name: openingBalance
  type: number
- description: ''
  name: closingBalance
  type: number
provider_name: BNY Mellon
provider_slug: bank-of-new-york-mellon
schema_file: json-schema/balance-schema.json
slug: balance
tags:
- Asset Servicing
- Banking
- Institutional Banking
- Payments
- Treasury
- Wire Transfers
title: Balance
---
