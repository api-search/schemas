---
description: An Activepieces automation flow
layout: schema
name: Flow
properties_list:
- description: Unique flow identifier
  name: id
  type: string
- description: Creation timestamp
  name: created
  type: string
- description: Last updated timestamp
  name: updated
  type: string
- description: Associated project ID
  name: projectId
  type: string
- description: External ID for the flow
  name: externalId
  type: string
- description: Human-readable flow name
  name: displayName
  type: string
- description: Flow status
  name: status
  type: string
- description: Folder ID if organized in a folder
  name: folderId
  type: string
- description: ID of the published version
  name: publishedVersionId
  type: string
provider_name: Activepieces
provider_slug: activepieces
schema_file: json-schema/activepieces-flow-schema.json
slug: activepieces-flow
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-flow-schema.json\",\n  \"title\": \"Flow\",\n  \"description\": \"An Activepieces automation flow\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique flow identifier\",\n      \"example\": \"flow-abc123\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Creation timestamp\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last updated timestamp\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated project ID\",\n      \"example\": \"project-xyz789\"\n \
  \   },\n    \"externalId\": {\n      \"type\": \"string\",\n      \"description\": \"External ID for the flow\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable flow name\",\n      \"example\": \"Send Welcome Email\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ENABLED\",\n        \"DISABLED\"\n      ],\n      \"description\": \"Flow status\",\n      \"example\": \"ENABLED\"\n    },\n    \"folderId\": {\n      \"type\": \"string\",\n      \"description\": \"Folder ID if organized in a folder\"\n    },\n    \"publishedVersionId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the published version\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-flow-schema.json
tags:
- Automation
- No-Code
- Open Source
- Workflow
- AI Agents
- MCP
title: Flow
---
