---
description: Represents an order for products and services.
layout: schema
name: Order
properties_list:
- description: Unique ID for this order.
  name: id
  type: string
- description: The ID of the seller location that this order is associated with.
  name: location_id
  type: string
- description: Current state of the order.
  name: state
  type: string
- description: Version number for optimistic concurrency control.
  name: version
  type: integer
- description: Total amount for the order.
  name: total_money
  type: object
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Block
provider_slug: block
schema_file: json-schema/block-order-schema.json
slug: block-order
tags:
- Commerce
- Cryptocurrency
- eCommerce
- Fintech
- Payments
- Point Of Sale
- Square
title: Order
---
