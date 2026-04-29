---
description: ''
layout: schema
name: Artifact
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: node_id
  type: string
- description: The name of the artifact.
  name: name
  type: string
- description: The size in bytes of the artifact.
  name: size_in_bytes
  type: integer
- description: ''
  name: url
  type: string
- description: ''
  name: archive_download_url
  type: string
- description: ''
  name: expired
  type: boolean
- description: ''
  name: created_at
  type: string
- description: ''
  name: expires_at
  type: string
- description: ''
  name: updated_at
  type: string
- description: ''
  name: workflow_run
  type: object
provider_name: GitHub Actions
provider_slug: github-actions
schema_file: json-schema/github-actions-artifact-schema.json
slug: github-actions-artifact
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Artifact\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"node_id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the artifact.\"\n    },\n    \"size_in_bytes\": {\n      \"type\": \"integer\",\n      \"description\": \"The size in bytes of the artifact.\"\n    },\n    \"url\": {\n      \"type\": \"string\"\n    },\n    \"archive_download_url\": {\n      \"type\": \"string\"\n    },\n    \"expired\": {\n      \"type\": \"boolean\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\n    },\n    \"expires_at\": {\n      \"type\": \"string\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\n    },\n    \"workflow_run\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/json-schema/github-actions-artifact-schema.json
tags: []
title: Artifact
---
