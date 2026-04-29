---
description: BounceStatistics schema from AhaSend API
layout: schema
name: BounceStatistics
properties_list:
- description: Start time of the statistics bucket
  name: from_timestamp
  type: string
- description: End time of the statistics bucket
  name: to_timestamp
  type: string
- description: Bounce count per bounce classification
  name: bounces
  type: array
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-bounce-statistics-schema.json
slug: openapi-v2-bounce-statistics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-bounce-statistics-schema.json\",\n  \"title\": \"BounceStatistics\",\n  \"description\": \"BounceStatistics schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"from_timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Start time of the statistics bucket\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"to_timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"End time of the statistics bucket\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"bounces\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Bounce\"\n      },\n      \"description\": \"Bounce count per bounce classification\",\n      \"example\":\
  \ [\n        {\n          \"classification\": \"example_value\",\n          \"count\": 1\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"from_timestamp\",\n    \"to_timestamp\",\n    \"bounces\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-bounce-statistics-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: BounceStatistics
---
