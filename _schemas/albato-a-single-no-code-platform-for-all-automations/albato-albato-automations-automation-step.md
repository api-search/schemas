---
description: A step in an automation workflow
layout: schema
name: AutomationStep
properties_list:
- description: App identifier
  name: app
  type: string
- description: Step type (trigger, action, condition, delay)
  name: type
  type: string
- description: Trigger or action event
  name: event
  type: string
- description: Step configuration
  name: config
  type: object
provider_name: Albato A Single No Code Platform For All Automations
provider_slug: albato-a-single-no-code-platform-for-all-automations
schema_file: json-schema/albato-albato-automations-automation-step-schema.json
slug: albato-albato-automations-automation-step
source_filename: albato-albato-automations-automation-step-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/albato-a-single-no-code-platform-for-all-automations/refs/heads/main/json-schema/albato-albato-automations-automation-step-schema.json\",\n  \"title\": \"AutomationStep\",\n  \"description\": \"A step in an automation workflow\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"app\": {\n      \"type\": \"string\",\n      \"description\": \"App identifier\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Step type (trigger, action, condition, delay)\"\n    },\n    \"event\": {\n      \"type\": \"string\",\n      \"description\": \"Trigger or action event\"\n    },\n    \"config\": {\n      \"type\": \"object\",\n      \"description\": \"Step configuration\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/albato-a-single-no-code-platform-for-all-automations/refs/heads/main/json-schema/albato-albato-automations-automation-step-schema.json
tags:
- No-Code Automation
- Workflow Automation
- App Integration
- Embedded iPaaS
- Integrations
- Webhooks
title: AutomationStep
---
