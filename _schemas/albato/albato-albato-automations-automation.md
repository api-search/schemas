---
description: A multi-step automation workflow
layout: schema
name: Automation
properties_list:
- description: ''
  name: id
  type: string
- description: Automation display name
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: active or inactive
  name: status
  type: string
- description: ''
  name: trigger_count
  type: integer
- description: ''
  name: success_count
  type: integer
- description: ''
  name: error_count
  type: integer
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Albato
provider_slug: albato
schema_file: json-schema/albato-albato-automations-automation-schema.json
slug: albato-albato-automations-automation
source_filename: albato-albato-automations-automation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/albato/refs/heads/main/json-schema/albato-albato-automations-automation-schema.json\",\n  \"title\": \"Automation\",\n  \"description\": \"A multi-step automation workflow\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Automation display name\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"active or inactive\"\n    },\n    \"trigger_count\": {\n      \"type\": \"integer\"\n    },\n    \"success_count\": {\n      \"type\": \"integer\"\n    },\n    \"error_count\": {\n      \"type\": \"integer\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updated_at\": {\n      \"type\"\
  : \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/albato/refs/heads/main/json-schema/albato-albato-automations-automation-schema.json
tags:
- No-Code Automation
- Workflow Automation
- Embedded iPaaS
- App Integration
- Integrations
- Webhooks
- White-Label
title: Automation
---
