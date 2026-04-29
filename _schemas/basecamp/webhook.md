---
description: ''
layout: schema
name: Webhook
properties_list:
- description: Webhook ID
  name: id
  type: integer
- description: Whether this webhook is currently active
  name: active
  type: boolean
- description: Timestamp when the webhook was created
  name: created_at
  type: string
- description: Timestamp when the webhook was last updated
  name: updated_at
  type: string
- description: HTTPS URL where Basecamp sends event notifications
  name: payload_url
  type: string
- description: Resource types that trigger this webhook
  name: types
  type: array
- description: API URL for this webhook
  name: url
  type: string
- description: Web URL for this webhook configuration
  name: app_url
  type: string
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/webhook-schema.json
slug: webhook
source_filename: webhook-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/webhook-schema.json\",\n  \"title\": \"Webhook\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Webhook ID\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this webhook is currently active\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the webhook was created\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the webhook was last updated\"\n    },\n    \"payload_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"HTTPS URL where Basecamp sends event notifications\"\n    },\n    \"types\": {\n      \"type\": \"array\"\
  ,\n      \"description\": \"Resource types that trigger this webhook\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"API URL for this webhook\"\n    },\n    \"app_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Web URL for this webhook configuration\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/webhook-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: Webhook
---
