---
description: Request body for updating a flow
layout: schema
name: UpdateFlowRequest
properties_list:
- description: New flow name
  name: displayName
  type: string
- description: Flow status
  name: status
  type: string
- description: Move to this folder
  name: folderId
  type: string
provider_name: Activepieces
provider_slug: activepieces
schema_file: json-schema/activepieces-update-flow-request-schema.json
slug: activepieces-update-flow-request
source_filename: activepieces-update-flow-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-update-flow-request-schema.json\",\n  \"title\": \"UpdateFlowRequest\",\n  \"description\": \"Request body for updating a flow\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"New flow name\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ENABLED\",\n        \"DISABLED\"\n      ],\n      \"description\": \"Flow status\"\n    },\n    \"folderId\": {\n      \"type\": \"string\",\n      \"description\": \"Move to this folder\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-update-flow-request-schema.json
tags:
- Automation
- No-Code
- Open Source
- Workflow
- AI Agents
- MCP
title: UpdateFlowRequest
---
