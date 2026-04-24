---
description: Account balance information
layout: schema
name: Balance
properties_list:
- description: Account identifier
  name: accountId
  type: string
- description: Current ledger balance
  name: ledgerBalance
  type: number
- description: Available balance for transactions
  name: availableBalance
  type: number
- description: Collected balance after float
  name: collectedBalance
  type: number
- description: Balance currency (ISO 4217)
  name: currency
  type: string
- description: Balance as of timestamp
  name: asOfDate
  type: string
provider_name: Bank of America
provider_slug: bank-of-america
schema_file: json-schema/balance-schema.json
slug: balance
tags:
- Banking
- Corporate Banking
- Finance
- Payments
- Treasury
- CashPro
title: Balance
---
