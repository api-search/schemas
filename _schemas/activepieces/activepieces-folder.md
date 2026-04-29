---
description: A folder for organizing flows
layout: schema
name: Folder
properties_list:
- description: Folder ID
  name: id
  type: string
- description: ''
  name: created
  type: string
- description: ''
  name: updated
  type: string
- description: Folder display name
  name: displayName
  type: string
- description: Project ID
  name: projectId
  type: string
provider_name: Activepieces
provider_slug: activepieces
schema_file: json-schema/activepieces-folder-schema.json
slug: activepieces-folder
source_filename: activepieces-folder-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-folder-schema.json\",\n  \"title\": \"Folder\",\n  \"description\": \"A folder for organizing flows\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Folder ID\",\n      \"example\": \"folder-abc123\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Folder display name\",\n      \"example\": \"Production Flows\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"Project ID\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-folder-schema.json
tags:
- Automation
- No-Code
- Open Source
- Workflow
- AI Agents
- MCP
title: Folder
---
