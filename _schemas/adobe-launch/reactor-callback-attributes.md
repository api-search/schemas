---
description: ''
layout: schema
name: CallbackAttributes
properties_list:
- description: The HTTPS URL to send callback messages to.
  name: url
  type: string
- description: The audit event types that trigger the callback.
  name: subscriptions
  type: array
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Adobe Launch
provider_slug: adobe-launch
schema_file: json-schema/reactor-callback-attributes-schema.json
slug: reactor-callback-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CallbackAttributes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The HTTPS URL to send callback messages to.\"\n    },\n    \"subscriptions\": {\n      \"type\": \"array\",\n      \"description\": \"The audit event types that trigger the callback.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/json-schema/reactor-callback-attributes-schema.json
tags:
- Data Collection
- Edge Network
- Event Forwarding
- Marketing Technology
- Tag Management
title: CallbackAttributes
---
