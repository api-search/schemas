---
description: A configured webhook for Vendr event notifications
layout: schema
name: Webhook
properties_list:
- description: Unique webhook identifier
  name: id
  type: string
- description: Webhook endpoint URL
  name: url
  type: string
- description: Subscribed event types
  name: events
  type: array
- description: Whether the webhook is active
  name: active
  type: boolean
provider_name: Blissfully
provider_slug: blissfully
schema_file: json-schema/blissfully-webhook-schema.json
slug: blissfully-webhook
source_filename: blissfully-webhook-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blissfully/refs/heads/main/json-schema/blissfully-webhook-schema.json\",\n  \"title\": \"Webhook\",\n  \"description\": \"A configured webhook for Vendr event notifications\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique webhook identifier\",\n      \"example\": \"webhook-500123\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Webhook endpoint URL\",\n      \"example\": \"https://example.com/webhook\"\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"description\": \"Subscribed event types\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"pricing.updated\"\n      ]\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether\
  \ the webhook is active\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"url\",\n    \"events\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blissfully/refs/heads/main/json-schema/blissfully-webhook-schema.json
tags:
- Procurement
- SaaS Discovery
- SaaS Management
- Software Procurement
- Spend Optimization
- Vendor Management
title: Webhook
---
