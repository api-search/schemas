---
description: Bank account details
layout: schema
name: Account
properties_list:
- description: Avaloq account ID
  name: id
  type: string
- description: IBAN or account number
  name: accountNumber
  type: string
- description: Account display name
  name: accountName
  type: string
- description: ISO 4217 currency code
  name: currency
  type: string
- description: Current balance
  name: balance
  type: number
- description: Available balance after holds
  name: availableBalance
  type: number
- description: ''
  name: status
  type: string
- description: Owning customer ID
  name: customerId
  type: string
- description: ''
  name: openedDate
  type: string
- description: ''
  name: accountType
  type: string
provider_name: Avaloq
provider_slug: avaloq
schema_file: json-schema/banking-account-schema.json
slug: banking-account
tags:
- Banking
- Digital Banking
- Financial Services
- Fintech
- Payments
- Wealth Management
title: Account
---
