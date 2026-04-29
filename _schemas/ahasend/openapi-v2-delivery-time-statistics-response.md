---
description: DeliveryTimeStatisticsResponse schema from AhaSend API
layout: schema
name: DeliveryTimeStatisticsResponse
properties_list:
- description: Object type identifier
  name: object
  type: string
- description: Array of delivery time statistics
  name: data
  type: array
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-delivery-time-statistics-response-schema.json
slug: openapi-v2-delivery-time-statistics-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-delivery-time-statistics-response-schema.json\",\n  \"title\": \"DeliveryTimeStatisticsResponse\",\n  \"description\": \"DeliveryTimeStatisticsResponse schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"list\"\n      ],\n      \"description\": \"Object type identifier\",\n      \"example\": \"list\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DeliveryTimeStatistics\"\n      },\n      \"description\": \"Array of delivery time statistics\",\n      \"example\": [\n        {\n          \"from_timestamp\": \"2025-03-15T14:30:00Z\",\n          \"to_timestamp\": \"2025-03-15T14:30:00Z\",\n          \"avg_delivery_time\": 1.0,\n          \"\
  delivered_count\": 1,\n          \"delivery_times\": [\n            {}\n          ]\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"object\",\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-delivery-time-statistics-response-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: DeliveryTimeStatisticsResponse
---
