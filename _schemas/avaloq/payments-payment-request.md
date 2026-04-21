---
description: Payment instruction request
layout: schema
name: PaymentRequest
properties_list:
- description: Source account ID
  name: debtorAccountId
  type: string
- description: Destination IBAN
  name: creditorIban
  type: string
- description: Beneficiary name
  name: creditorName
  type: string
- description: Payment amount
  name: amount
  type: number
- description: ISO 4217 currency code
  name: currency
  type: string
- description: Payment reference
  name: remittanceInfo
  type: string
- description: ''
  name: paymentType
  type: string
- description: ''
  name: executionDate
  type: string
provider_name: Avaloq
provider_slug: avaloq
schema_file: json-schema/payments-payment-request-schema.json
slug: payments-payment-request
tags:
- Banking
- Digital Banking
- Financial Services
- Fintech
- Payments
- Wealth Management
title: PaymentRequest
---
