---
description: A BNY Mellon treasury account
layout: schema
name: Account
properties_list:
- description: Unique account identifier
  name: accountId
  type: string
- description: Account number (masked)
  name: accountNumber
  type: string
- description: Account name
  name: accountName
  type: string
- description: Account type
  name: accountType
  type: string
- description: Account currency (ISO 4217)
  name: currency
  type: string
- description: Account status
  name: status
  type: string
- description: BNY Mellon bank code
  name: bankCode
  type: string
provider_name: BNY Mellon
provider_slug: bank-of-new-york-mellon
schema_file: json-schema/account-schema.json
slug: account
tags:
- Asset Servicing
- Banking
- Institutional Banking
- Payments
- Treasury
- Wire Transfers
title: Account
---
