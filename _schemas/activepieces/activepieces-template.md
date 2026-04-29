---
description: A flow template for reuse
layout: schema
name: Template
properties_list:
- description: Template ID
  name: id
  type: string
- description: ''
  name: created
  type: string
- description: Template name
  name: name
  type: string
- description: Template description
  name: description
  type: string
- description: Template tags
  name: tags
  type: array
provider_name: Activepieces
provider_slug: activepieces
schema_file: json-schema/activepieces-template-schema.json
slug: activepieces-template
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-template-schema.json\",\n  \"title\": \"Template\",\n  \"description\": \"A flow template for reuse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Template ID\",\n      \"example\": \"template-abc123\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Template name\",\n      \"example\": \"Lead Notification Template\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Template description\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Template tags\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-template-schema.json
tags:
- Automation
- No-Code
- Open Source
- Workflow
- AI Agents
- MCP
title: Template
---
