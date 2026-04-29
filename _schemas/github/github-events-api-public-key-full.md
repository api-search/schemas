---
description: public-key-full from GitHub API
layout: schema
name: public-key-full
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: key
  type: string
- description: ''
  name: user_id
  type: integer
- description: ''
  name: repository_id
  type: integer
- description: ''
  name: url
  type: string
- description: ''
  name: title
  type: string
- description: ''
  name: read_only
  type: boolean
- description: ''
  name: verified
  type: boolean
- description: ''
  name: created_at
  type: string
- description: ''
  name: added_by
  type: string
- description: ''
  name: last_used
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-events-api-public-key-full-schema.json
slug: github-events-api-public-key-full
source_filename: github-events-api-public-key-full-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-events-api-public-key-full-schema.json\",\n  \"title\": \"public-key-full\",\n  \"description\": \"public-key-full from GitHub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 42\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"user_id\": {\n      \"nullable\": true,\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"repository_id\": {\n      \"nullable\": true,\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 42\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"example\"\
  : \"Example Title\"\n    },\n    \"read_only\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"verified\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"added_by\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"example\": \"example_value\"\n    },\n    \"last_used\": {\n      \"nullable\": true,\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"key\",\n    \"url\",\n    \"title\",\n    \"verified\",\n    \"created_at\",\n    \"read_only\",\n    \"last_used\",\n    \"user_id\",\n    \"repository_id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-events-api-public-key-full-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: public-key-full
---
