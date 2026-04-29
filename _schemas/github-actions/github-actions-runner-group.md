---
description: ''
layout: schema
name: RunnerGroup
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: visibility
  type: string
- description: ''
  name: default
  type: boolean
- description: ''
  name: runners_url
  type: string
- description: ''
  name: inherited
  type: boolean
- description: ''
  name: allows_public_repositories
  type: boolean
provider_name: GitHub Actions
provider_slug: github-actions
schema_file: json-schema/github-actions-runner-group-schema.json
slug: github-actions-runner-group
source_filename: github-actions-runner-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RunnerGroup\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"visibility\": {\n      \"type\": \"string\"\n    },\n    \"default\": {\n      \"type\": \"boolean\"\n    },\n    \"runners_url\": {\n      \"type\": \"string\"\n    },\n    \"inherited\": {\n      \"type\": \"boolean\"\n    },\n    \"allows_public_repositories\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/json-schema/github-actions-runner-group-schema.json
tags: []
title: RunnerGroup
---
