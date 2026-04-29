---
description: An app connection for authentication
layout: schema
name: Connection
properties_list:
- description: ''
  name: id
  type: string
- description: App identifier
  name: app
  type: string
- description: Connection display name
  name: name
  type: string
- description: Authentication type
  name: auth_type
  type: string
- description: Connection status
  name: status
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: last_used_at
  type: string
provider_name: Albato A Single No Code Platform For All Automations
provider_slug: albato-a-single-no-code-platform-for-all-automations
schema_file: json-schema/albato-albato-connections-connection-schema.json
slug: albato-albato-connections-connection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/albato-a-single-no-code-platform-for-all-automations/refs/heads/main/json-schema/albato-albato-connections-connection-schema.json\",\n  \"title\": \"Connection\",\n  \"description\": \"An app connection for authentication\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"app\": {\n      \"type\": \"string\",\n      \"description\": \"App identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Connection display name\"\n    },\n    \"auth_type\": {\n      \"type\": \"string\",\n      \"description\": \"Authentication type\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Connection status\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"last_used_at\": {\n    \
  \  \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/albato-a-single-no-code-platform-for-all-automations/refs/heads/main/json-schema/albato-albato-connections-connection-schema.json
tags:
- No-Code Automation
- Workflow Automation
- App Integration
- Embedded iPaaS
- Integrations
- Webhooks
title: Connection
---
