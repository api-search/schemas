---
description: Represents a cached dependency entry in GitHub Actions.
layout: schema
name: GitHub Actions Cache Entry
properties_list:
- description: Unique identifier of the cache entry.
  name: id
  type: integer
- description: The Git reference for the cache entry.
  name: ref
  type: string
- description: The cache key used to identify the cache entry.
  name: key
  type: string
- description: The version of the cache entry.
  name: version
  type: string
- description: The date and time the cache was last accessed.
  name: last_accessed_at
  type: string
- description: The date and time the cache was created.
  name: created_at
  type: string
- description: The size of the cache entry in bytes.
  name: size_in_bytes
  type: integer
provider_name: GitHub Actions
provider_slug: github-actions
schema_file: json-schema/github-actions-cache-schema.json
slug: github-actions-cache
source_filename: github-actions-cache-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.github.com/actions/cache-entry.json\",\n  \"title\": \"GitHub Actions Cache Entry\",\n  \"description\": \"Represents a cached dependency entry in GitHub Actions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier of the cache entry.\"\n    },\n    \"ref\": {\n      \"type\": \"string\",\n      \"description\": \"The Git reference for the cache entry.\",\n      \"examples\": [\"refs/heads/main\"]\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The cache key used to identify the cache entry.\",\n      \"examples\": [\"node-modules-abc123\", \"pip-cache-linux-x64-def456\"]\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the cache entry.\"\n    },\n    \"last_accessed_at\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date-time\",\n      \"description\": \"The date and time the cache was last accessed.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the cache was created.\"\n    },\n    \"size_in_bytes\": {\n      \"type\": \"integer\",\n      \"description\": \"The size of the cache entry in bytes.\",\n      \"minimum\": 0\n    }\n  },\n  \"required\": [\"id\", \"ref\", \"key\", \"version\", \"last_accessed_at\", \"created_at\", \"size_in_bytes\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/json-schema/github-actions-cache-schema.json
tags: []
title: GitHub Actions Cache Entry
---
