---
description: A step in an automation workflow
layout: schema
name: AutomationStep
properties_list:
- description: App identifier
  name: app
  type: string
- description: trigger, action, condition, or delay
  name: type
  type: string
- description: Event name
  name: event
  type: string
- description: ''
  name: config
  type: object
provider_name: Albato
provider_slug: albato
schema_file: json-schema/albato-albato-automations-automation-step-schema.json
slug: albato-albato-automations-automation-step
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/albato/refs/heads/main/json-schema/albato-albato-automations-automation-step-schema.json\",\n  \"title\": \"AutomationStep\",\n  \"description\": \"A step in an automation workflow\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"app\": {\n      \"type\": \"string\",\n      \"description\": \"App identifier\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"trigger, action, condition, or delay\"\n    },\n    \"event\": {\n      \"type\": \"string\",\n      \"description\": \"Event name\"\n    },\n    \"config\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/albato/refs/heads/main/json-schema/albato-albato-automations-automation-step-schema.json
tags:
- No-Code Automation
- Workflow Automation
- Embedded iPaaS
- App Integration
- Integrations
- Webhooks
- White-Label
title: AutomationStep
---
