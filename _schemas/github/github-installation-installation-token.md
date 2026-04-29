---
description: Authentication token for a GitHub App installed on a user or org.
layout: schema
name: installation-token
properties_list:
- description: ''
  name: token
  type: string
- description: ''
  name: expires_at
  type: string
- description: ''
  name: permissions
  type: object
- description: ''
  name: repository_selection
  type: string
- description: ''
  name: repositories
  type: array
- description: ''
  name: single_file
  type: string
- description: ''
  name: has_multiple_single_files
  type: boolean
- description: ''
  name: single_file_paths
  type: array
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-installation-installation-token-schema.json
slug: github-installation-installation-token
source_filename: github-installation-installation-token-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-installation-installation-token-schema.json\",\n  \"title\": \"installation-token\",\n  \"description\": \"Authentication token for a GitHub App installed on a user or org.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"expires_at\": {\n      \"type\": \"string\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"permissions\": {\n      \"$ref\": \"#/components/schemas/app-permissions\"\n    },\n    \"repository_selection\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"all\",\n        \"selected\"\n      ],\n      \"example\": \"all\"\n    },\n    \"repositories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/repository\"\n      }\n\
  \    },\n    \"single_file\": {\n      \"type\": \"string\",\n      \"example\": \"README.md\"\n    },\n    \"has_multiple_single_files\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"single_file_paths\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"config.yml\",\n        \".github/issue_TEMPLATE.md\"\n      ]\n    }\n  },\n  \"required\": [\n    \"token\",\n    \"expires_at\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-installation-installation-token-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: installation-token
---
