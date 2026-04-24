---
description: An account transaction record
layout: schema
name: Transaction
properties_list:
- description: Unique transaction identifier
  name: transactionId
  type: string
- description: Account the transaction belongs to
  name: accountId
  type: string
- description: Transaction type (debit, credit)
  name: type
  type: string
- description: Transaction amount
  name: amount
  type: number
- description: Transaction currency
  name: currency
  type: string
- description: Transaction description or memo
  name: description
  type: string
- description: Bank reference number
  name: referenceNumber
  type: string
- description: Value date of the transaction
  name: valueDate
  type: string
- description: Post date of the transaction
  name: postDate
  type: string
- description: Transaction status
  name: status
  type: string
provider_name: Bank of America
provider_slug: bank-of-america
schema_file: json-schema/transaction-schema.json
slug: transaction
tags:
- Banking
- Corporate Banking
- Finance
- Payments
- Treasury
- CashPro
title: Transaction
---
