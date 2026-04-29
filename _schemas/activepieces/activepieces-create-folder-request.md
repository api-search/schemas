---
description: CreateFolderRequest schema from Activepieces API
layout: schema
name: CreateFolderRequest
properties_list:
- description: Folder name
  name: displayName
  type: string
- description: Project ID
  name: projectId
  type: string
provider_name: Activepieces
provider_slug: activepieces
schema_file: json-schema/activepieces-create-folder-request-schema.json
slug: activepieces-create-folder-request
source_filename: activepieces-create-folder-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-create-folder-request-schema.json\",\n  \"title\": \"CreateFolderRequest\",\n  \"description\": \"CreateFolderRequest schema from Activepieces API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Folder name\",\n      \"example\": \"My Folder\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"Project ID\"\n    }\n  },\n  \"required\": [\n    \"displayName\",\n    \"projectId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-create-folder-request-schema.json
tags:
- Automation
- No-Code
- Open Source
- Workflow
- AI Agents
- MCP
title: CreateFolderRequest
---
