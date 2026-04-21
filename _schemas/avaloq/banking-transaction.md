---
description: Bank account transaction
layout: schema
name: Transaction
properties_list:
- description: Transaction ID
  name: id
  type: string
- description: ''
  name: accountId
  type: string
- description: Transaction amount (positive=credit, negative=debit)
  name: amount
  type: number
- description: ''
  name: currency
  type: string
- description: ''
  name: valueDate
  type: string
- description: ''
  name: bookingDate
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: counterpartyName
  type: string
- description: ''
  name: counterpartyIban
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: status
  type: string
provider_name: Avaloq
provider_slug: avaloq
schema_file: json-schema/banking-transaction-schema.json
slug: banking-transaction
tags:
- Banking
- Digital Banking
- Financial Services
- Fintech
- Payments
- Wealth Management
title: Transaction
---
