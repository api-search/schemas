---
description: Payment initiation request
layout: schema
name: PaymentRequest
properties_list:
- description: Payment type (WIRE, ACH_CREDIT, ACH_DEBIT, SWIFT, CHIPS)
  name: paymentType
  type: string
- description: ''
  name: amount
  type: number
- description: ''
  name: currency
  type: string
- description: ''
  name: debitAccountId
  type: string
- description: ''
  name: valueDate
  type: string
- description: ''
  name: creditorName
  type: string
- description: ''
  name: creditorAccountNumber
  type: string
- description: ''
  name: creditorBankCode
  type: string
- description: ''
  name: creditorSwiftCode
  type: string
- description: ''
  name: remittanceInfo
  type: string
- description: ''
  name: clientReference
  type: string
provider_name: BNY Mellon
provider_slug: bank-of-new-york-mellon
schema_file: json-schema/paymentrequest-schema.json
slug: paymentrequest
tags:
- Asset Servicing
- Banking
- Institutional Banking
- Payments
- Treasury
- Wire Transfers
title: PaymentRequest
---
