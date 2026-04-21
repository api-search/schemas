---
description: POSTransaction schema from Aramark Marko API
layout: schema
name: POSTransaction
properties_list:
- description: Transaction identifier
  name: transactionId
  type: string
- description: Location identifier
  name: locationId
  type: string
- description: Transaction amount in USD
  name: amount
  type: number
- description: Number of items in the transaction
  name: items
  type: integer
- description: Transaction timestamp (ISO 8601)
  name: timestamp
  type: string
- description: Payment method used
  name: paymentMethod
  type: string
provider_name: Aramark
provider_slug: aramark
schema_file: json-schema/marko-api-pos-transaction-schema.json
slug: marko-api-pos-transaction
tags:
- Food Services
- Facilities Management
- Uniform Services
- Data Platform
- Fortune 500
title: POSTransaction
---
