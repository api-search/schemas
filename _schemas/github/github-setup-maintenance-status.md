---
description: maintenance-status from GitHub API
layout: schema
name: maintenance-status
properties_list:
- description: ''
  name: status
  type: string
- description: ''
  name: scheduled_time
  type: string
- description: ''
  name: connection_services
  type: array
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-setup-maintenance-status-schema.json
slug: github-setup-maintenance-status
source_filename: github-setup-maintenance-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-setup-maintenance-status-schema.json\",\n  \"title\": \"maintenance-status\",\n  \"description\": \"maintenance-status from GitHub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"example\": \"open\"\n    },\n    \"scheduled_time\": {\n      \"type\": \"string\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"connection_services\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"number\": {\n            \"type\": \"integer\"\n          }\n        },\n        \"required\": [\n          \"name\",\n          \"number\"\n        ]\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-setup-maintenance-status-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: maintenance-status
---
