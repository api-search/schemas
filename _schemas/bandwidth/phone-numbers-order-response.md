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
source_filename: phone-numbers-order-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-order-response-schema.json\",\n  \"title\": \"OrderResponse\",\n  \"description\": \"Response containing order details\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"orderId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the order\"\n    },\n    \"orderStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"RECEIVED\",\n        \"PROCESSING\",\n        \"COMPLETE\",\n        \"PARTIAL\",\n        \"FAILED\"\n      ],\n      \"description\": \"The current status of the order\"\n    },\n    \"orderCreateDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the order was created\"\n    },\n    \"completedQuantity\": {\n      \"type\": \"integer\",\n      \"description\": \"\
  Number of phone numbers successfully ordered\"\n    },\n    \"failedQuantity\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of phone numbers that failed to order\"\n    },\n    \"completedNumbers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of successfully ordered phone numbers\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-order-response-schema.json
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
