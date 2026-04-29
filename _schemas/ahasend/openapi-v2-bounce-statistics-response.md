---
description: BounceStatisticsResponse schema from AhaSend API
layout: schema
name: BounceStatisticsResponse
properties_list:
- description: Object type identifier
  name: object
  type: string
- description: Array of bounce statistics
  name: data
  type: array
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-bounce-statistics-response-schema.json
slug: openapi-v2-bounce-statistics-response
source_filename: openapi-v2-bounce-statistics-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-bounce-statistics-response-schema.json\",\n  \"title\": \"BounceStatisticsResponse\",\n  \"description\": \"BounceStatisticsResponse schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"list\"\n      ],\n      \"description\": \"Object type identifier\",\n      \"example\": \"list\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/BounceStatistics\"\n      },\n      \"description\": \"Array of bounce statistics\",\n      \"example\": [\n        {\n          \"from_timestamp\": \"2025-03-15T14:30:00Z\",\n          \"to_timestamp\": \"2025-03-15T14:30:00Z\",\n          \"bounces\": [\n            {}\n          ]\n        }\n      ]\n    }\n\
  \  },\n  \"required\": [\n    \"object\",\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-bounce-statistics-response-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: BounceStatisticsResponse
---
