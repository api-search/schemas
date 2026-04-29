---
description: A record of a Power Automate flow run execution.
layout: schema
name: FlowRun
properties_list:
- description: The unique identifier of the flow run.
  name: name
  type: string
- description: The fully qualified resource ID of the flow run.
  name: id
  type: string
- description: The resource type.
  name: type
  type: string
provider_name: Microsoft Power Platform APIs
provider_slug: power-platform
schema_file: json-schema/power-platform-flow-run-schema.json
slug: power-platform-flow-run
source_filename: power-platform-flow-run-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FlowRun\",\n  \"type\": \"object\",\n  \"description\": \"A record of a Power Automate flow run execution.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the flow run.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The fully qualified resource ID of the flow run.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-platform/refs/heads/main/json-schema/power-platform-flow-run-schema.json
tags:
- Business Applications
- Copilot Studio
- Dataverse
- Low-Code
- Microsoft
- No-Code
- Power Pages
- Power Platform
title: FlowRun
---
