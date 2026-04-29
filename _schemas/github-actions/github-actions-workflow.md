---
description: ''
layout: schema
name: Workflow
properties_list:
- description: Unique identifier of the workflow.
  name: id
  type: integer
- description: ''
  name: node_id
  type: string
- description: The name of the workflow.
  name: name
  type: string
- description: The path of the workflow file relative to the root of the repository.
  name: path
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: html_url
  type: string
- description: ''
  name: badge_url
  type: string
provider_name: GitHub Actions
provider_slug: github-actions
schema_file: json-schema/github-actions-workflow-schema.json
slug: github-actions-workflow
source_filename: github-actions-workflow-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Workflow\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier of the workflow.\"\n    },\n    \"node_id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the workflow.\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"The path of the workflow file relative to the root of the repository.\"\n    },\n    \"state\": {\n      \"type\": \"string\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\n    },\n    \"url\": {\n      \"type\": \"string\"\n    },\n    \"html_url\": {\n      \"type\": \"string\"\n    },\n    \"badge_url\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/json-schema/github-actions-workflow-schema.json
tags: []
title: Workflow
---
