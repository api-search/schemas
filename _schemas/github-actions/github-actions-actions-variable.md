---
description: ''
layout: schema
name: ActionsVariable
properties_list:
- description: The name of the variable.
  name: name
  type: string
- description: The value of the variable.
  name: value
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: GitHub Actions
provider_slug: github-actions
schema_file: json-schema/github-actions-actions-variable-schema.json
slug: github-actions-actions-variable
source_filename: github-actions-actions-variable-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ActionsVariable\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the variable.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the variable.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/json-schema/github-actions-actions-variable-schema.json
tags: []
title: ActionsVariable
---
