---
description: FolderList schema from Activepieces API
layout: schema
name: FolderList
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: next
  type: string
- description: ''
  name: previous
  type: string
provider_name: Activepieces
provider_slug: activepieces
schema_file: json-schema/activepieces-folder-list-schema.json
slug: activepieces-folder-list
source_filename: activepieces-folder-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-folder-list-schema.json\",\n  \"title\": \"FolderList\",\n  \"description\": \"FolderList schema from Activepieces API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Folder\"\n      }\n    },\n    \"next\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"previous\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-folder-list-schema.json
tags:
- Automation
- No-Code
- Open Source
- Workflow
- AI Agents
- MCP
title: FolderList
---
