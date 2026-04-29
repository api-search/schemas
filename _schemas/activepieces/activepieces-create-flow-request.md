---
description: Request body for creating a flow
layout: schema
name: CreateFlowRequest
properties_list:
- description: Flow display name
  name: displayName
  type: string
- description: Project ID to create flow in
  name: projectId
  type: string
- description: Optional folder ID
  name: folderId
  type: string
- description: Optional template to base the flow on
  name: templateId
  type: string
- description: Custom metadata
  name: metadata
  type: object
provider_name: Activepieces
provider_slug: activepieces
schema_file: json-schema/activepieces-create-flow-request-schema.json
slug: activepieces-create-flow-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-create-flow-request-schema.json\",\n  \"title\": \"CreateFlowRequest\",\n  \"description\": \"Request body for creating a flow\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Flow display name\",\n      \"example\": \"My New Flow\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"Project ID to create flow in\",\n      \"example\": \"project-xyz789\"\n    },\n    \"folderId\": {\n      \"type\": \"string\",\n      \"description\": \"Optional folder ID\"\n    },\n    \"templateId\": {\n      \"type\": \"string\",\n      \"description\": \"Optional template to base the flow on\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Custom metadata\"\n\
  \    }\n  },\n  \"required\": [\n    \"displayName\",\n    \"projectId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-create-flow-request-schema.json
tags:
- Automation
- No-Code
- Open Source
- Workflow
- AI Agents
- MCP
title: CreateFlowRequest
---
