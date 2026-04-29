---
description: A Power Automate cloud flow.
layout: schema
name: Flow
properties_list:
- description: The unique name or ID of the flow.
  name: name
  type: string
- description: The full resource ID of the flow.
  name: id
  type: string
- description: The resource type.
  name: type
  type: string
- description: ''
  name: properties
  type: object
provider_name: Microsoft Power Automate
provider_slug: microsoft-power-automate
schema_file: json-schema/power-automate-management-api-flow-schema.json
slug: power-automate-management-api-flow
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-power-automate/refs/heads/main/json-schema/power-automate-management-api-flow-schema.json\",\n  \"title\": \"Flow\",\n  \"description\": \"A Power Automate cloud flow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": { \"type\": \"string\", \"description\": \"The unique name or ID of the flow.\" },\n    \"id\": { \"type\": \"string\", \"description\": \"The full resource ID of the flow.\" },\n    \"type\": { \"type\": \"string\", \"description\": \"The resource type.\" },\n    \"properties\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayName\": { \"type\": \"string\", \"description\": \"The display name of the flow.\" },\n        \"state\": { \"type\": \"string\", \"enum\": [\"Started\", \"Stopped\", \"Suspended\"] },\n        \"createdTime\": { \"type\": \"string\", \"format\": \"date-time\"\
  \ },\n        \"lastModifiedTime\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"templateName\": { \"type\": \"string\" },\n        \"flowTriggerUri\": { \"type\": \"string\" },\n        \"installationStatus\": { \"type\": \"string\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-automate/refs/heads/main/json-schema/power-automate-management-api-flow-schema.json
tags:
- Automation
- Business Process
- Integration
- Low-Code
- Microsoft
- Power Platform
- RPA
- Workflow
title: Flow
---
