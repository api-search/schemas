---
description: A domestic payment initiation request for the Barclays Payment Initiation API.
layout: schema
name: PaymentRequest
properties_list:
- description: Unique identifier for the payment instruction assigned by the PISP.
  name: instructionIdentification
  type: string
- description: End-to-end reference for the payment.
  name: endToEndIdentification
  type: string
- description: ''
  name: instructedAmount
  type: object
- description: ''
  name: creditorAccount
  type: object
- description: ''
  name: remittanceInformation
  type: object
provider_name: Barclays
provider_slug: barclays
schema_file: json-schema/payment-schema.json
slug: payment
tags:
- Banking
- Credit Cards
- Finance
- Open Banking
- Payments
- PSD2
- UK Banking
title: PaymentRequest
---
