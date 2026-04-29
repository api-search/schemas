---
description: rate-limit from GitHub API
layout: schema
name: rate-limit
properties_list:
- description: ''
  name: limit
  type: integer
- description: ''
  name: remaining
  type: integer
- description: ''
  name: reset
  type: integer
- description: ''
  name: used
  type: integer
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-rate-limit--rate-limit-schema.json
slug: github-rate-limit--rate-limit
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-rate-limit--rate-limit-schema.json\",\n  \"title\": \"rate-limit\",\n  \"description\": \"rate-limit from GitHub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"limit\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"remaining\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"reset\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"used\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    }\n  },\n  \"required\": [\n    \"limit\",\n    \"remaining\",\n    \"reset\",\n    \"used\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-rate-limit--rate-limit-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: rate-limit
---
