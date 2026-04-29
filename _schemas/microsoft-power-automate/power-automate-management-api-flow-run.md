---
description: A flow run representing a single execution of a flow.
layout: schema
name: FlowRun
properties_list:
- description: The unique ID of the flow run.
  name: name
  type: string
- description: The full resource ID.
  name: id
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: properties
  type: object
provider_name: Microsoft Power Automate
provider_slug: microsoft-power-automate
schema_file: json-schema/power-automate-management-api-flow-run-schema.json
slug: power-automate-management-api-flow-run
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-power-automate/refs/heads/main/json-schema/power-automate-management-api-flow-run-schema.json\",\n  \"title\": \"FlowRun\",\n  \"description\": \"A flow run representing a single execution of a flow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": { \"type\": \"string\", \"description\": \"The unique ID of the flow run.\" },\n    \"id\": { \"type\": \"string\", \"description\": \"The full resource ID.\" },\n    \"type\": { \"type\": \"string\" },\n    \"properties\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"startTime\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"endTime\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"status\": { \"type\": \"string\", \"enum\": [\"Running\", \"Succeeded\", \"Failed\", \"Cancelled\", \"Waiting\", \"Suspended\"] },\n       \
  \ \"code\": { \"type\": \"string\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-automate/refs/heads/main/json-schema/power-automate-management-api-flow-run-schema.json
tags:
- Automation
- Business Process
- Integration
- Low-Code
- Microsoft
- Power Platform
- RPA
- Workflow
title: FlowRun
---
