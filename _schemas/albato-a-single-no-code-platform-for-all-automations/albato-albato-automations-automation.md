---
description: An automation workflow connecting multiple apps
layout: schema
name: Automation
properties_list:
- description: Unique automation identifier
  name: id
  type: string
- description: Automation display name
  name: name
  type: string
- description: Automation description
  name: description
  type: string
- description: Automation status (active/inactive)
  name: status
  type: string
- description: Total trigger count
  name: trigger_count
  type: integer
- description: Successful execution count
  name: success_count
  type: integer
- description: Error count
  name: error_count
  type: integer
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Albato A Single No Code Platform For All Automations
provider_slug: albato-a-single-no-code-platform-for-all-automations
schema_file: json-schema/albato-albato-automations-automation-schema.json
slug: albato-albato-automations-automation
source_filename: albato-albato-automations-automation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/albato-a-single-no-code-platform-for-all-automations/refs/heads/main/json-schema/albato-albato-automations-automation-schema.json\",\n  \"title\": \"Automation\",\n  \"description\": \"An automation workflow connecting multiple apps\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique automation identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Automation display name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Automation description\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Automation status (active/inactive)\"\n    },\n    \"trigger_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total trigger count\"\n    },\n    \"success_count\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Successful execution count\"\n    },\n    \"error_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Error count\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/albato-a-single-no-code-platform-for-all-automations/refs/heads/main/json-schema/albato-albato-automations-automation-schema.json
tags:
- No-Code Automation
- Workflow Automation
- App Integration
- Embedded iPaaS
- Integrations
- Webhooks
title: Automation
---
