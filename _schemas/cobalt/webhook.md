---
description: A webhook subscription for receiving real-time notifications when events occur in Cobalt.
layout: schema
name: Webhook
properties_list:
- description: Webhook ID.
  name: _id
  type: string
- description: The webhook notification URL.
  name: webhook_url
  type: string
- description: Subscribed event names.
  name: webhook_events
  type: array
- description: The linked account ID.
  name: linked_account_id
  type: string
provider_name: Cobalt
provider_slug: cobalt
schema_file: json-schema/webhook.json
slug: webhook
source_filename: webhook.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cobalt/refs/heads/main/json-schema/webhook.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Webhook\",\n  \"description\": \"A webhook subscription for receiving real-time notifications when events occur in Cobalt.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Webhook ID.\"\n    },\n    \"webhook_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The webhook notification URL.\"\n    },\n    \"webhook_events\": {\n      \"type\": \"array\",\n      \"description\": \"Subscribed event names.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"linked_account_id\": {\n      \"type\": \"string\",\n      \"description\": \"The linked account ID.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cobalt/refs/heads/main/json-schema/webhook.json
tags:
- Automation
- Embedded iPaaS
- Integrations
title: Webhook
---
