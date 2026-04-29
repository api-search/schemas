---
description: UpdateRouteRequest schema from AhaSend API
layout: schema
name: UpdateRouteRequest
properties_list:
- description: Route name
  name: name
  type: string
- description: Webhook URL for the route
  name: url
  type: string
- description: Recipient filter
  name: recipient
  type: string
- description: Whether to include attachments in webhooks
  name: attachments
  type: boolean
- description: Whether to include headers in webhooks
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
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-update-route-request-schema.json
slug: openapi-v2-update-route-request
source_filename: openapi-v2-update-route-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-update-route-request-schema.json\",\n  \"title\": \"UpdateRouteRequest\",\n  \"description\": \"UpdateRouteRequest schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"maxLength\": 255,\n      \"nullable\": true,\n      \"description\": \"Route name\",\n      \"example\": \"Example Name\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"nullable\": true,\n      \"description\": \"Webhook URL for the route\",\n      \"example\": \"https://example.com\"\n    },\n    \"recipient\": {\n      \"type\": \"string\",\n      \"maxLength\": 255,\n      \"nullable\": true,\n      \"description\": \"Recipient filter\",\n      \"example\": \"example_value\"\n    },\n    \"attachments\": {\n      \"\
  type\": \"boolean\",\n      \"nullable\": true,\n      \"description\": \"Whether to include attachments in webhooks\",\n      \"example\": true\n    },\n    \"headers\": {\n      \"type\": \"boolean\",\n      \"nullable\": true,\n      \"description\": \"Whether to include headers in webhooks\",\n      \"example\": true\n    },\n    \"group_by_message_id\": {\n      \"type\": \"boolean\",\n      \"nullable\": true,\n      \"description\": \"Whether to group by message ID\",\n      \"example\": true\n    },\n    \"strip_replies\": {\n      \"type\": \"boolean\",\n      \"nullable\": true,\n      \"description\": \"Whether to strip reply content\",\n      \"example\": true\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"nullable\": true,\n      \"description\": \"Whether the route is enabled\",\n      \"example\": true\n    }\n  },\n  \"example\": {\n    \"name\": \"Updated Support Route\",\n    \"enabled\": false\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-update-route-request-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: UpdateRouteRequest
---
