---
description: Represents a payment processed by Square.
layout: schema
name: Payment
properties_list:
- description: Unique ID for this payment.
  name: id
  type: string
- description: Indicates whether the payment is APPROVED, COMPLETED, CANCELED, or FAILED.
  name: status
  type: string
- description: The source type for this payment.
  name: source_type
  type: string
- description: ''
  name: amount_money
  type: object
- description: ''
  name: total_money
  type: object
- description: The ID of the location associated with the payment.
  name: location_id
  type: string
- description: The timestamp of when the payment was created.
  name: created_at
  type: string
- description: The timestamp of when the payment was last updated.
  name: updated_at
  type: string
provider_name: Block
provider_slug: block
schema_file: json-schema/block-payment-schema.json
slug: block-payment
tags:
- Commerce
- Cryptocurrency
- eCommerce
- Fintech
- Payments
- Point Of Sale
- Square
title: Payment
---
