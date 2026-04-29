---
description: ''
layout: schema
name: WebhookCreateRequest
properties_list:
- description: HTTPS URL to receive webhook event notifications
  name: payload_url
  type: string
- description: Resource types to subscribe to. Omit to subscribe to all types.
  name: types
  type: array
- description: Whether the webhook should be active upon creation
  name: active
  type: boolean
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/webhookcreaterequest-schema.json
slug: webhookcreaterequest
source_filename: webhookcreaterequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/webhookcreaterequest-schema.json\",\n  \"title\": \"WebhookCreateRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"payload_url\"\n  ],\n  \"properties\": {\n    \"payload_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"HTTPS URL to receive webhook event notifications\"\n    },\n    \"types\": {\n      \"type\": \"array\",\n      \"description\": \"Resource types to subscribe to. Omit to subscribe to all types.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"Message\",\n          \"Todo\",\n          \"Todolist\",\n          \"Document\",\n          \"Comment\",\n          \"Kanban::Card\",\n          \"Schedule::Entry\",\n          \"Vault\",\n          \"Upload\",\n          \"Client::Forward\",\n          \"Client::Correspondence\",\n         \
  \ \"Question\",\n          \"Question::Answer\",\n          \"Inbox::Forward\"\n        ]\n      }\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the webhook should be active upon creation\",\n      \"default\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/webhookcreaterequest-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: WebhookCreateRequest
---
