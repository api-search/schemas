---
description: Represents an eCommerce order synced to the Brevo platform for revenue attribution, purchase behavior tracking, and automated marketing workflows.
layout: schema
name: Brevo eCommerce Order
properties_list:
- description: Unique identifier of the order from the merchant's system.
  name: id
  type: string
- description: Email address of the customer who placed the order.
  name: email
  type: string
- description: Current status of the order in the fulfillment workflow.
  name: status
  type: string
- description: Total order amount including shipping, tax, and item prices.
  name: amount
  type: number
- description: List of products included in the order.
  name: products
  type: array
- description: UTC date-time when the order was created.
  name: createdAt
  type: string
- description: UTC date-time when the order was last updated.
  name: updatedAt
  type: string
- description: Coupon codes applied to the order.
  name: coupons
  type: array
provider_name: brevo
provider_slug: brevo
schema_file: json-schema/brevo-order-schema.json
slug: brevo-order
tags: []
title: Brevo eCommerce Order
---
