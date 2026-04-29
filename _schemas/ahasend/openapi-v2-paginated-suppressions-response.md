---
description: PaginatedSuppressionsResponse schema from AhaSend API
layout: schema
name: PaginatedSuppressionsResponse
properties_list:
- description: Object type identifier
  name: object
  type: string
- description: Array of suppressions
  name: data
  type: array
- description: ''
  name: pagination
  type: object
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-paginated-suppressions-response-schema.json
slug: openapi-v2-paginated-suppressions-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-paginated-suppressions-response-schema.json\",\n  \"title\": \"PaginatedSuppressionsResponse\",\n  \"description\": \"PaginatedSuppressionsResponse schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"list\"\n      ],\n      \"description\": \"Object type identifier\",\n      \"example\": \"list\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Suppression\"\n      },\n      \"description\": \"Array of suppressions\",\n      \"example\": [\n        {\n          \"object\": \"suppression\",\n          \"id\": \"500123\",\n          \"created_at\": \"2025-03-15T14:30:00Z\",\n          \"updated_at\": \"2025-03-15T14:30:00Z\",\n          \"\
  email\": \"user@example.com\"\n        }\n      ]\n    },\n    \"pagination\": {\n      \"$ref\": \"#/components/schemas/PaginationInfo\"\n    }\n  },\n  \"required\": [\n    \"object\",\n    \"data\",\n    \"pagination\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-paginated-suppressions-response-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: PaginatedSuppressionsResponse
---
