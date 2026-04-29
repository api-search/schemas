---
description: An embedded team representing a customer account
layout: schema
name: Team
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: external_id
  type: string
- description: ''
  name: plan
  type: string
- description: ''
  name: active_automations
  type: integer
- description: ''
  name: transaction_count
  type: integer
- description: ''
  name: created_at
  type: string
provider_name: Albato
provider_slug: albato
schema_file: json-schema/albato-albato-embedded-team-schema.json
slug: albato-albato-embedded-team
source_filename: albato-albato-embedded-team-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/albato/refs/heads/main/json-schema/albato-albato-embedded-team-schema.json\",\n  \"title\": \"Team\",\n  \"description\": \"An embedded team representing a customer account\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"external_id\": {\n      \"type\": \"string\"\n    },\n    \"plan\": {\n      \"type\": \"string\"\n    },\n    \"active_automations\": {\n      \"type\": \"integer\"\n    },\n    \"transaction_count\": {\n      \"type\": \"integer\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/albato/refs/heads/main/json-schema/albato-albato-embedded-team-schema.json
tags:
- No-Code Automation
- Workflow Automation
- Embedded iPaaS
- App Integration
- Integrations
- Webhooks
- White-Label
title: Team
---
