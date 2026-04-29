---
description: CreateTemplateRequest schema from Activepieces API
layout: schema
name: CreateTemplateRequest
properties_list:
- description: Template name
  name: name
  type: string
- description: Template description
  name: description
  type: string
- description: ''
  name: tags
  type: array
provider_name: Activepieces
provider_slug: activepieces
schema_file: json-schema/activepieces-create-template-request-schema.json
slug: activepieces-create-template-request
source_filename: activepieces-create-template-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-create-template-request-schema.json\",\n  \"title\": \"CreateTemplateRequest\",\n  \"description\": \"CreateTemplateRequest schema from Activepieces API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Template name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Template description\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-create-template-request-schema.json
tags:
- Automation
- No-Code
- Open Source
- Workflow
- AI Agents
- MCP
title: CreateTemplateRequest
---
