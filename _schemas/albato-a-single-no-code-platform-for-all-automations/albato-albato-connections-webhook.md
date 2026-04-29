---
description: An inbound webhook endpoint
layout: schema
name: Webhook
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: Webhook endpoint URL
  name: url
  type: string
- description: ''
  name: created_at
  type: string
provider_name: Albato A Single No Code Platform For All Automations
provider_slug: albato-a-single-no-code-platform-for-all-automations
schema_file: json-schema/albato-albato-connections-webhook-schema.json
slug: albato-albato-connections-webhook
source_filename: albato-albato-connections-webhook-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/albato-a-single-no-code-platform-for-all-automations/refs/heads/main/json-schema/albato-albato-connections-webhook-schema.json\",\n  \"title\": \"Webhook\",\n  \"description\": \"An inbound webhook endpoint\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Webhook endpoint URL\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/albato-a-single-no-code-platform-for-all-automations/refs/heads/main/json-schema/albato-albato-connections-webhook-schema.json
tags:
- No-Code Automation
- Workflow Automation
- App Integration
- Embedded iPaaS
- Integrations
- Webhooks
title: Webhook
---
