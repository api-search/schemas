---
description: Paginated list of flows
layout: schema
name: FlowList
properties_list:
- description: Array of flows
  name: data
  type: array
- description: Cursor to next page
  name: next
  type: string
- description: Cursor to previous page
  name: previous
  type: string
provider_name: Activepieces
provider_slug: activepieces
schema_file: json-schema/activepieces-flow-list-schema.json
slug: activepieces-flow-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-flow-list-schema.json\",\n  \"title\": \"FlowList\",\n  \"description\": \"Paginated list of flows\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Flow\"\n      },\n      \"description\": \"Array of flows\"\n    },\n    \"next\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Cursor to next page\"\n    },\n    \"previous\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Cursor to previous page\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-flow-list-schema.json
tags:
- Automation
- No-Code
- Open Source
- Workflow
- AI Agents
- MCP
title: FlowList
---
