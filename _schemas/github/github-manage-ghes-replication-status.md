---
description: ghes-replication-status from GitHub API
layout: schema
name: ghes-replication-status
properties_list:
- description: ''
  name: status
  type: object
- description: ''
  name: nodes
  type: array
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-manage-ghes-replication-status-schema.json
slug: github-manage-ghes-replication-status
source_filename: github-manage-ghes-replication-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-manage-ghes-replication-status-schema.json\",\n  \"title\": \"ghes-replication-status\",\n  \"description\": \"ghes-replication-status from GitHub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"$ref\": \"#/components/schemas/ghes-replication-status-indicator\"\n    },\n    \"nodes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"hostname\": {\n            \"type\": \"string\"\n          },\n          \"status\": {\n            \"$ref\": \"#/components/schemas/ghes-replication-status-indicator\"\n          },\n          \"services\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"status\": {\n  \
  \                \"$ref\": \"#/components/schemas/ghes-replication-status-indicator\"\n                },\n                \"name\": {\n                  \"type\": \"string\"\n                },\n                \"details\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-manage-ghes-replication-status-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: ghes-replication-status
---
