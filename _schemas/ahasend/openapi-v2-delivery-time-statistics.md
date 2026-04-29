---
description: DeliveryTimeStatistics schema from AhaSend API
layout: schema
name: DeliveryTimeStatistics
properties_list:
- description: Start time of the statistics bucket
  name: from_timestamp
  type: string
- description: End time of the statistics bucket
  name: to_timestamp
  type: string
- description: Average delivery time in seconds
  name: avg_delivery_time
  type: number
- description: Number of messages
  name: delivered_count
  type: integer
- description: ''
  name: delivery_times
  type: array
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-delivery-time-statistics-schema.json
slug: openapi-v2-delivery-time-statistics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-delivery-time-statistics-schema.json\",\n  \"title\": \"DeliveryTimeStatistics\",\n  \"description\": \"DeliveryTimeStatistics schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"from_timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Start time of the statistics bucket\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"to_timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"End time of the statistics bucket\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"avg_delivery_time\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Average delivery time in seconds\",\n      \"example\": 1.0\n    },\n    \"delivered_count\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Number of messages\",\n      \"example\": 1\n    },\n    \"delivery_times\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DeliveryTime\",\n        \"description\": \"Delivery times per recipient domain\"\n      },\n      \"example\": [\n        {\n          \"recipient_domain\": \"mail.example.com\",\n          \"delivery_time\": 1.0\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"from_timestamp\",\n    \"to_timestamp\",\n    \"avg_delivery_time\",\n    \"delivered_count\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-delivery-time-statistics-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: DeliveryTimeStatistics
---
