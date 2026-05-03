---
description: Schema for a Sanity webhook configuration for receiving event-driven content notifications.
layout: schema
name: Sanity Webhook
properties_list:
- description: Unique webhook identifier (assigned by Sanity)
  name: id
  type: string
- description: Human-readable webhook name
  name: name
  type: string
- description: Target URL to receive webhook POST requests
  name: url
  type: string
- description: Dataset to watch for changes
  name: dataset
  type: string
- description: GROQ filter expression to match specific documents
  name: filter
  type: string
- description: GROQ projection to shape the webhook payload
  name: projection
  type: string
- description: Events that trigger the webhook
  name: 'on'
  type: array
- description: Optional secret for signing webhook payloads (HMAC-SHA256)
  name: secret
  type: string
- description: Whether the webhook is currently disabled
  name: isDisabled
  type: boolean
- description: ''
  name: createdAt
  type: string
provider_name: Sanity
provider_slug: sanity
schema_file: json-schema/sanity-webhook-schema.json
slug: sanity-webhook
source_filename: sanity-webhook-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/sanity/json-schema/webhook.json\",\n  \"title\": \"Sanity Webhook\",\n  \"description\": \"Schema for a Sanity webhook configuration for receiving event-driven content notifications.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"url\", \"dataset\", \"on\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique webhook identifier (assigned by Sanity)\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable webhook name\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Target URL to receive webhook POST requests\"\n    },\n    \"dataset\": {\n      \"type\": \"string\",\n      \"description\": \"Dataset to watch for changes\",\n      \"examples\": [\"production\", \"staging\"]\n    },\n    \"filter\": {\n     \
  \ \"type\": \"string\",\n      \"description\": \"GROQ filter expression to match specific documents\",\n      \"examples\": [\"_type == 'post'\", \"_type in ['post', 'page']\"]\n    },\n    \"projection\": {\n      \"type\": \"string\",\n      \"description\": \"GROQ projection to shape the webhook payload\"\n    },\n    \"on\": {\n      \"type\": \"array\",\n      \"description\": \"Events that trigger the webhook\",\n      \"minItems\": 1,\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"create\", \"update\", \"delete\"]\n      }\n    },\n    \"secret\": {\n      \"type\": \"string\",\n      \"description\": \"Optional secret for signing webhook payloads (HMAC-SHA256)\"\n    },\n    \"isDisabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the webhook is currently disabled\",\n      \"default\": false\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sanity/refs/heads/main/json-schema/sanity-webhook-schema.json
tags:
- Headless CMS
- Content Management
- GROQ
- Real-Time
- Structured Content
- Developer Platform
title: Sanity Webhook
---
