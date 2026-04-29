---
description: UserList schema from Activepieces API
layout: schema
name: UserList
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
schema_file: json-schema/activepieces-user-list-schema.json
slug: activepieces-user-list
source_filename: activepieces-user-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-user-list-schema.json\",\n  \"title\": \"UserList\",\n  \"description\": \"UserList schema from Activepieces API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/User\"\n      }\n    },\n    \"next\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"previous\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-user-list-schema.json
tags:
- Automation
- No-Code
- Open Source
- Workflow
- AI Agents
- MCP
title: UserList
---
