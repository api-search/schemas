---
description: Payment transaction response
layout: schema
name: PaymentResponse
properties_list:
- description: Unique payment identifier
  name: paymentId
  type: string
- description: Client-provided reference
  name: clientReferenceId
  type: string
- description: Payment status
  name: status
  type: string
- description: Payment type
  name: paymentType
  type: string
- description: ''
  name: amount
  type: number
- description: ''
  name: currency
  type: string
- description: ''
  name: valueDate
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
- description: Additional status information
  name: statusMessage
  type: string
provider_name: Bank of America
provider_slug: bank-of-america
schema_file: json-schema/paymentresponse-schema.json
slug: paymentresponse
tags:
- Banking
- Corporate Banking
- Finance
- Payments
- Treasury
- CashPro
title: PaymentResponse
---
