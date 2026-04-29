---
description: ''
layout: schema
name: Template
properties_list:
- description: Template ID
  name: id
  type: integer
- description: Template status
  name: status
  type: string
- description: Timestamp when the template was created
  name: created_at
  type: string
- description: Timestamp when the template was last updated
  name: updated_at
  type: string
- description: Template name
  name: name
  type: string
- description: Template description
  name: description
  type: string
- description: API URL for this template
  name: url
  type: string
- description: Web URL for this template
  name: app_url
  type: string
- description: Tools available in this template
  name: dock
  type: array
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/template-schema.json
slug: template
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/template-schema.json\",\n  \"title\": \"Template\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"status\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Template ID\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Template status\",\n      \"enum\": [\n        \"active\",\n        \"archived\",\n        \"trashed\"\n      ]\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the template was created\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the template was last updated\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Template name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Template description\",\n      \"nullable\": true\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"API URL for this template\"\n    },\n    \"app_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Web URL for this template\"\n    },\n    \"dock\": {\n      \"type\": \"array\",\n      \"description\": \"Tools available in this template\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DockItem\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/template-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: Template
---
