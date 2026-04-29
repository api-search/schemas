---
description: TemplateList schema from Activepieces API
layout: schema
name: TemplateList
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
schema_file: json-schema/activepieces-template-list-schema.json
slug: activepieces-template-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-template-list-schema.json\",\n  \"title\": \"TemplateList\",\n  \"description\": \"TemplateList schema from Activepieces API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Template\"\n      }\n    },\n    \"next\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"previous\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-template-list-schema.json
tags:
- Automation
- No-Code
- Open Source
- Workflow
- AI Agents
- MCP
title: TemplateList
---
