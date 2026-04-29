---
description: PaginatedMessagesResponse schema from AhaSend API
layout: schema
name: PaginatedMessagesResponse
properties_list:
- description: Object type identifier
  name: object
  type: string
- description: Array of message summaries (content and content_parsed fields omitted for performance)
  name: data
  type: array
- description: ''
  name: pagination
  type: object
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-paginated-messages-response-schema.json
slug: openapi-v2-paginated-messages-response
source_filename: openapi-v2-paginated-messages-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-paginated-messages-response-schema.json\",\n  \"title\": \"PaginatedMessagesResponse\",\n  \"description\": \"PaginatedMessagesResponse schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"list\"\n      ],\n      \"description\": \"Object type identifier\",\n      \"example\": \"list\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MessageSummary\"\n      },\n      \"description\": \"Array of message summaries (content and content_parsed fields omitted for performance)\",\n      \"example\": [\n        {\n          \"object\": \"message\",\n          \"created_at\": \"2025-03-15T14:30:00Z\",\n          \"updated_at\": \"2025-03-15T14:30:00Z\"\
  ,\n          \"sent_at\": \"2025-03-15T14:30:00Z\",\n          \"delivered_at\": \"2025-03-15T14:30:00Z\"\n        }\n      ]\n    },\n    \"pagination\": {\n      \"$ref\": \"#/components/schemas/PaginationInfo\"\n    }\n  },\n  \"required\": [\n    \"object\",\n    \"data\",\n    \"pagination\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-paginated-messages-response-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: PaginatedMessagesResponse
---
