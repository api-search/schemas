---
description: A workspace in the Tray.ai platform used to organize users, projects, and workflows into sub-categories.
layout: schema
name: Tray.ai Workspace
properties_list:
- description: Unique workspace identifier
  name: id
  type: string
- description: Display name of the workspace
  name: name
  type: string
- description: Description of the workspace purpose
  name: description
  type: string
- description: Timestamp when the workspace was created
  name: createdAt
  type: string
provider_name: Tray.ai
provider_slug: tray-ai
schema_file: json-schema/workspace.json
slug: workspace
source_filename: workspace.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/json-schema/workspace.json\",\n  \"title\": \"Tray.ai Workspace\",\n  \"description\": \"A workspace in the Tray.ai platform used to organize users, projects, and workflows into sub-categories.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique workspace identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the workspace\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the workspace purpose\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the workspace was created\"\n    }\n  },\n  \"required\": [\"id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/json-schema/workspace.json
tags:
- Automation
- Integration
- iPaaS
title: Tray.ai Workspace
---
