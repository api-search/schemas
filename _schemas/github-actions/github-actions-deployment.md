---
description: ''
layout: schema
name: Deployment
properties_list:
- description: ''
  name: url
  type: string
- description: ''
  name: id
  type: integer
- description: ''
  name: node_id
  type: string
- description: ''
  name: task
  type: string
- description: ''
  name: environment
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: GitHub Actions
provider_slug: github-actions
schema_file: json-schema/github-actions-deployment-schema.json
slug: github-actions-deployment
source_filename: github-actions-deployment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Deployment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"node_id\": {\n      \"type\": \"string\"\n    },\n    \"task\": {\n      \"type\": \"string\"\n    },\n    \"environment\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/json-schema/github-actions-deployment-schema.json
tags: []
title: Deployment
---
