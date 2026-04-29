---
description: ''
layout: schema
name: ActionsPublicKey
properties_list:
- description: The identifier for the key.
  name: key_id
  type: string
- description: The Base64 encoded public key.
  name: key
  type: string
provider_name: GitHub Actions
provider_slug: github-actions
schema_file: json-schema/github-actions-actions-public-key-schema.json
slug: github-actions-actions-public-key
source_filename: github-actions-actions-public-key-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ActionsPublicKey\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key_id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier for the key.\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The Base64 encoded public key.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/json-schema/github-actions-actions-public-key-schema.json
tags: []
title: ActionsPublicKey
---
