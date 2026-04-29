---
description: global-hook from GitHub API
layout: schema
name: global-hook
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: id
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: active
  type: boolean
- description: ''
  name: events
  type: array
- description: ''
  name: config
  type: object
- description: ''
  name: updated_at
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: ping_url
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-openapi-global-hook-schema.json
slug: github-openapi-global-hook
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-openapi-global-hook-schema.json\",\n  \"title\": \"global-hook\",\n  \"description\": \"global-hook from GitHub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"User\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"octocat\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"config\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\"\n        },\n        \"content_type\": {\n          \"type\": \"string\"\n        },\n\
  \        \"insecure_ssl\": {\n          \"type\": \"string\"\n        },\n        \"secret\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"ping_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-openapi-global-hook-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: global-hook
---
