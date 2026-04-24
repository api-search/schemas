---
description: Payment initiation request
layout: schema
name: PaymentRequest
properties_list:
- description: Payment type (ACH_CREDIT, WIRE, SWIFT, CHECK, RTP, etc.)
  name: paymentType
  type: string
- description: Payment amount
  name: amount
  type: number
- description: Payment currency (ISO 4217)
  name: currency
  type: string
- description: Account to debit
  name: debitAccountId
  type: string
- description: Requested value date (ISO 8601)
  name: valueDate
  type: string
- description: Client reference number
  name: reference
  type: string
- description: Payment memo or description
  name: memo
  type: string
- description: ''
  name: beneficiary
  type: object
provider_name: Bank of America
provider_slug: bank-of-america
schema_file: json-schema/paymentrequest-schema.json
slug: paymentrequest
tags:
- Banking
- Corporate Banking
- Finance
- Payments
- Treasury
- CashPro
title: PaymentRequest
---
