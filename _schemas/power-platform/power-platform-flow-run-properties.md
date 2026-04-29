---
description: Properties of a flow run.
layout: schema
name: FlowRunProperties
properties_list:
- description: The timestamp when the flow run started.
  name: startTime
  type: string
- description: The timestamp when the flow run ended. Null if still running.
  name: endTime
  type: '[''string'', ''null'']'
- description: The current status of the flow run.
  name: status
  type: string
- description: Correlation information for the flow run.
  name: correlation
  type: object
- description: Information about the trigger that initiated the flow run.
  name: trigger
  type: object
provider_name: Microsoft Power Platform APIs
provider_slug: power-platform
schema_file: json-schema/power-platform-flow-run-properties-schema.json
slug: power-platform-flow-run-properties
source_filename: power-platform-flow-run-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FlowRunProperties\",\n  \"type\": \"object\",\n  \"description\": \"Properties of a flow run.\",\n  \"properties\": {\n    \"startTime\": {\n      \"type\": \"string\",\n      \"description\": \"The timestamp when the flow run started.\"\n    },\n    \"endTime\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The timestamp when the flow run ended. Null if still running.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the flow run.\"\n    },\n    \"correlation\": {\n      \"type\": \"object\",\n      \"description\": \"Correlation information for the flow run.\"\n    },\n    \"trigger\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the trigger that initiated the flow run.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-platform/refs/heads/main/json-schema/power-platform-flow-run-properties-schema.json
tags:
- Business Applications
- Copilot Studio
- Dataverse
- Low-Code
- Microsoft
- No-Code
- Power Pages
- Power Platform
title: FlowRunProperties
---
