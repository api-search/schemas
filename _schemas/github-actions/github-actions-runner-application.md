---
description: ''
layout: schema
name: RunnerApplication
properties_list:
- description: ''
  name: os
  type: string
- description: ''
  name: architecture
  type: string
- description: ''
  name: download_url
  type: string
- description: ''
  name: filename
  type: string
- description: ''
  name: temp_download_token
  type: string
- description: ''
  name: sha256_checksum
  type: string
provider_name: GitHub Actions
provider_slug: github-actions
schema_file: json-schema/github-actions-runner-application-schema.json
slug: github-actions-runner-application
source_filename: github-actions-runner-application-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RunnerApplication\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"os\": {\n      \"type\": \"string\"\n    },\n    \"architecture\": {\n      \"type\": \"string\"\n    },\n    \"download_url\": {\n      \"type\": \"string\"\n    },\n    \"filename\": {\n      \"type\": \"string\"\n    },\n    \"temp_download_token\": {\n      \"type\": \"string\"\n    },\n    \"sha256_checksum\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/json-schema/github-actions-runner-application-schema.json
tags: []
title: RunnerApplication
---
