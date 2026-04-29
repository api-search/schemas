---
description: Delivery tracking record for an order
layout: schema
name: Delivery
properties_list:
- description: Unique delivery identifier
  name: deliveryId
  type: string
- description: Associated order identifier
  name: orderId
  type: string
- description: Shipping carrier name
  name: carrier
  type: string
- description: Carrier tracking number
  name: trackingNumber
  type: string
- description: Current delivery status
  name: status
  type: string
- description: Estimated delivery date
  name: estimatedDelivery
  type: string
- description: Timestamp when the shipment was dispatched
  name: shippedAt
  type: string
provider_name: 3M
provider_slug: 3m
schema_file: json-schema/3m-partner-supplier-api-delivery-schema.json
slug: 3m-partner-supplier-api-delivery
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/3m/refs/heads/main/json-schema/3m-partner-supplier-api-delivery-schema.json\",\n  \"title\": \"Delivery\",\n  \"description\": \"Delivery tracking record for an order\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deliveryId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique delivery identifier\",\n      \"example\": \"DEL-11111\"\n    },\n    \"orderId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated order identifier\",\n      \"example\": \"ORD-67890\"\n    },\n    \"carrier\": {\n      \"type\": \"string\",\n      \"description\": \"Shipping carrier name\",\n      \"example\": \"UPS\"\n    },\n    \"trackingNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Carrier tracking number\",\n      \"example\": \"1Z999AA10123456784\"\n    },\n    \"status\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Current delivery status\",\n      \"enum\": [\n        \"pending\",\n        \"in-transit\",\n        \"out-for-delivery\",\n        \"delivered\",\n        \"exception\"\n      ],\n      \"example\": \"in-transit\"\n    },\n    \"estimatedDelivery\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Estimated delivery date\",\n      \"example\": \"2025-03-20\"\n    },\n    \"shippedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the shipment was dispatched\",\n      \"example\": \"2025-03-17T08:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/3m/refs/heads/main/json-schema/3m-partner-supplier-api-delivery-schema.json
tags:
- Industrial
- Manufacturing
- Supply Chain
title: Delivery
---
