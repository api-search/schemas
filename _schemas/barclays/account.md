---
description: A Barclays bank account as returned by the Open Banking Account Information API.
layout: schema
name: Account
properties_list:
- description: Unique identifier for the account.
  name: accountId
  type: string
- description: ISO 4217 currency code.
  name: currency
  type: string
- description: Type of the account.
  name: accountType
  type: string
- description: Sub-type of the account.
  name: accountSubType
  type: string
- description: Customer-assigned nickname for the account.
  name: nickname
  type: string
- description: ''
  name: account
  type: array
- description: ''
  name: balances
  type: array
provider_name: Barclays
provider_slug: barclays
schema_file: json-schema/account-schema.json
slug: account
tags:
- Banking
- Credit Cards
- Finance
- Open Banking
- Payments
- PSD2
- UK Banking
title: Account
---
