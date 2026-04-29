---
description: An Activepieces project
layout: schema
name: Project
properties_list:
- description: Project ID
  name: id
  type: string
- description: ''
  name: created
  type: string
- description: ''
  name: updated
  type: string
- description: Project display name
  name: displayName
  type: string
- description: Owner user ID
  name: ownerId
  type: string
- description: Platform ID
  name: platformId
  type: string
provider_name: Activepieces
provider_slug: activepieces
schema_file: json-schema/activepieces-project-schema.json
slug: activepieces-project
source_filename: activepieces-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-project-schema.json\",\n  \"title\": \"Project\",\n  \"description\": \"An Activepieces project\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Project ID\",\n      \"example\": \"project-abc123\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Project display name\",\n      \"example\": \"My Project\"\n    },\n    \"ownerId\": {\n      \"type\": \"string\",\n      \"description\": \"Owner user ID\"\n    },\n    \"platformId\": {\n      \"type\": \"string\",\n      \"description\": \"Platform ID\"\n    }\n \
  \ }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-project-schema.json
tags:
- Automation
- No-Code
- Open Source
- Workflow
- AI Agents
- MCP
title: Project
---
