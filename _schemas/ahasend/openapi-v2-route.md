---
description: Route schema from AhaSend API
layout: schema
name: Route
properties_list:
- description: Object type identifier
  name: object
  type: string
- description: Unique identifier for the route
  name: id
  type: string
- description: When the route was created
  name: created_at
  type: string
- description: When the route was last updated
  name: updated_at
  type: string
- description: Route name
  name: name
  type: string
- description: Webhook URL for the route
  name: url
  type: string
- description: Recipient filter
  name: recipient
  type: string
- description: Whether to include attachments in route payload
  name: attachments
  type: boolean
- description: Whether to include headers in route payload
  name: headers
  type: boolean
- description: Whether to group by message ID
  name: group_by_message_id
  type: boolean
- description: Whether to strip reply content
  name: strip_replies
  type: boolean
- description: Whether the route is enabled
  name: enabled
  type: boolean
- description: Number of successful calls
  name: success_count
  type: integer
- description: Number of unsuccessful calls
  name: error_count
  type: integer
- description: Number of consecutive failed calls
  name: errors_since_last_success
  type: integer
- description: When the route was last called
  name: last_request_at
  type: string
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-route-schema.json
slug: openapi-v2-route
source_filename: openapi-v2-route-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-route-schema.json\",\n  \"title\": \"Route\",\n  \"description\": \"Route schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"route\"\n      ],\n      \"description\": \"Object type identifier\",\n      \"example\": \"route\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the route\",\n      \"example\": \"500123\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the route was created\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"When the route was last updated\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Route name\",\n      \"example\": \"Example Name\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Webhook URL for the route\",\n      \"example\": \"https://example.com\"\n    },\n    \"recipient\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Recipient filter\",\n      \"example\": \"example_value\"\n    },\n    \"attachments\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to include attachments in route payload\",\n      \"example\": true\n    },\n    \"headers\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to include headers in route payload\",\n      \"example\": true\n    },\n    \"group_by_message_id\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to group by\
  \ message ID\",\n      \"example\": true\n    },\n    \"strip_replies\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to strip reply content\",\n      \"example\": true\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the route is enabled\",\n      \"example\": true\n    },\n    \"success_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of successful calls\",\n      \"example\": 1\n    },\n    \"error_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of unsuccessful calls\",\n      \"example\": 1\n    },\n    \"errors_since_last_success\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of consecutive failed calls\",\n      \"example\": 1\n    },\n    \"last_request_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the route was last called\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  },\n  \"\
  required\": [\n    \"object\",\n    \"id\",\n    \"created_at\",\n    \"updated_at\",\n    \"name\",\n    \"url\",\n    \"enabled\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-route-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: Route
---
