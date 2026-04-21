---
description: Response containing order details
layout: schema
name: OrderResponse
properties_list:
- description: The unique identifier for the order
  name: orderId
  type: string
- description: The current status of the order
  name: orderStatus
  type: string
- description: The date and time the order was created
  name: orderCreateDate
  type: string
- description: Number of phone numbers successfully ordered
  name: completedQuantity
  type: integer
- description: Number of phone numbers that failed to order
  name: failedQuantity
  type: integer
- description: List of successfully ordered phone numbers
  name: completedNumbers
  type: array
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/phone-numbers-order-response-schema.json
slug: phone-numbers-order-response
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: OrderResponse
---
