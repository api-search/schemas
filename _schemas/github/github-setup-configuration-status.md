---
description: configuration-status from GitHub API
layout: schema
name: configuration-status
properties_list:
- description: ''
  name: status
  type: string
- description: ''
  name: progress
  type: array
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-setup-configuration-status-schema.json
slug: github-setup-configuration-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-setup-configuration-status-schema.json\",\n  \"title\": \"configuration-status\",\n  \"description\": \"configuration-status from GitHub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"example\": \"open\"\n    },\n    \"progress\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"status\": {\n            \"type\": \"string\"\n          },\n          \"key\": {\n            \"type\": \"string\"\n          }\n        },\n        \"required\": [\n          \"status\",\n          \"key\"\n        ]\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-setup-configuration-status-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: configuration-status
---
