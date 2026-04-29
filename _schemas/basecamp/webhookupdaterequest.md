---
description: ''
layout: schema
name: WebhookUpdateRequest
properties_list:
- description: Updated HTTPS URL for event delivery
  name: payload_url
  type: string
- description: Updated list of subscribed resource types
  name: types
  type: array
- description: Whether the webhook should be active
  name: active
  type: boolean
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/webhookupdaterequest-schema.json
slug: webhookupdaterequest
source_filename: webhookupdaterequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/webhookupdaterequest-schema.json\",\n  \"title\": \"WebhookUpdateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"payload_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Updated HTTPS URL for event delivery\"\n    },\n    \"types\": {\n      \"type\": \"array\",\n      \"description\": \"Updated list of subscribed resource types\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the webhook should be active\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/webhookupdaterequest-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: WebhookUpdateRequest
---
