---
description: A Bank of America CashPro account
layout: schema
name: Account
properties_list:
- description: Unique account identifier
  name: accountId
  type: string
- description: Masked account number
  name: accountNumber
  type: string
- description: Account display name
  name: accountName
  type: string
- description: Account type (checking, savings, etc.)
  name: accountType
  type: string
- description: Account currency (ISO 4217)
  name: currency
  type: string
- description: ABA routing number
  name: routingNumber
  type: string
- description: Account status
  name: status
  type: string
- description: Date the account was opened
  name: openDate
  type: string
provider_name: Bank of America
provider_slug: bank-of-america
schema_file: json-schema/account-schema.json
slug: account
tags:
- Banking
- Corporate Banking
- Finance
- Payments
- Treasury
- CashPro
title: Account
---
