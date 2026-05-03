---
description: A webhook configured to receive real-time notifications for events such as user status updates from IDP and HRMS tools.
layout: schema
name: Zluri Webhook
properties_list:
- description: Unique identifier of the webhook.
  name: id
  type: string
- description: The URL that will receive webhook notifications.
  name: url
  type: string
- description: List of event types this webhook subscribes to.
  name: events
  type: array
- description: Current status of the webhook.
  name: status
  type: string
- description: When the webhook was created.
  name: created_at
  type: string
- description: When the webhook was last updated.
  name: updated_at
  type: string
provider_name: Zluri
provider_slug: zluri
schema_file: json-schema/webhook.json
slug: webhook
source_filename: webhook.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/zluri/refs/heads/main/json-schema/webhook.json\",\n  \"title\": \"Zluri Webhook\",\n  \"description\": \"A webhook configured to receive real-time notifications for events such as user status updates from IDP and HRMS tools.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the webhook.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL that will receive webhook notifications.\"\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of event types this webhook subscribes to.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the webhook.\",\n      \"enum\"\
  : [\"active\", \"inactive\"]\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the webhook was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the webhook was last updated.\"\n    }\n  },\n  \"required\": [\"id\", \"url\", \"events\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zluri/refs/heads/main/json-schema/webhook.json
tags:
- Access Management
- SaaS Management
title: Zluri Webhook
---
