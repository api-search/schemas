---
description: pre-receive-environment from GitHub API
layout: schema
name: pre-receive-environment
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: image_url
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: html_url
  type: string
- description: ''
  name: default_environment
  type: boolean
- description: ''
  name: created_at
  type: string
- description: ''
  name: hooks_count
  type: integer
- description: ''
  name: download
  type: object
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-openapi-pre-receive-environment-schema.json
slug: github-openapi-pre-receive-environment
source_filename: github-openapi-pre-receive-environment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-openapi-pre-receive-environment-schema.json\",\n  \"title\": \"pre-receive-environment\",\n  \"description\": \"pre-receive-environment from GitHub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"octocat\"\n    },\n    \"image_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"default_environment\": {\n      \"type\": \"boolean\",\n\
  \      \"example\": true\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"hooks_count\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"download\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\"\n        },\n        \"state\": {\n          \"type\": \"string\"\n        },\n        \"downloaded_at\": {\n          \"nullable\": true,\n          \"type\": \"string\"\n        },\n        \"message\": {\n          \"nullable\": true,\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-openapi-pre-receive-environment-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: pre-receive-environment
---
