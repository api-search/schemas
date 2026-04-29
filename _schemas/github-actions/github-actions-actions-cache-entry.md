---
description: ''
layout: schema
name: ActionsCacheEntry
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: ref
  type: string
- description: ''
  name: key
  type: string
- description: ''
  name: version
  type: string
- description: ''
  name: last_accessed_at
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: size_in_bytes
  type: integer
provider_name: GitHub Actions
provider_slug: github-actions
schema_file: json-schema/github-actions-actions-cache-entry-schema.json
slug: github-actions-actions-cache-entry
source_filename: github-actions-actions-cache-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ActionsCacheEntry\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"ref\": {\n      \"type\": \"string\"\n    },\n    \"key\": {\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"type\": \"string\"\n    },\n    \"last_accessed_at\": {\n      \"type\": \"string\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\n    },\n    \"size_in_bytes\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/json-schema/github-actions-actions-cache-entry-schema.json
tags: []
title: ActionsCacheEntry
---
