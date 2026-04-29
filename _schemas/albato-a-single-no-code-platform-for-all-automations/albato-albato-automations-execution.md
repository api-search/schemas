---
description: An automation execution record
layout: schema
name: Execution
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: automation_id
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: started_at
  type: string
- description: ''
  name: finished_at
  type: string
- description: ''
  name: error_message
  type: string
- description: ''
  name: steps_completed
  type: integer
provider_name: Albato A Single No Code Platform For All Automations
provider_slug: albato-a-single-no-code-platform-for-all-automations
schema_file: json-schema/albato-albato-automations-execution-schema.json
slug: albato-albato-automations-execution
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/albato-a-single-no-code-platform-for-all-automations/refs/heads/main/json-schema/albato-albato-automations-execution-schema.json\",\n  \"title\": \"Execution\",\n  \"description\": \"An automation execution record\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"automation_id\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"started_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"finished_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"error_message\": {\n      \"type\": \"string\"\n    },\n    \"steps_completed\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/albato-a-single-no-code-platform-for-all-automations/refs/heads/main/json-schema/albato-albato-automations-execution-schema.json
tags:
- No-Code Automation
- Workflow Automation
- App Integration
- Embedded iPaaS
- Integrations
- Webhooks
title: Execution
---
