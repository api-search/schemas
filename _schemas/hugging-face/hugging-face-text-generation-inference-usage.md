---
description: ''
layout: schema
name: Usage
properties_list:
- description: ''
  name: prompt_tokens
  type: integer
- description: ''
  name: completion_tokens
  type: integer
- description: ''
  name: total_tokens
  type: integer
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-text-generation-inference-usage-schema.json
slug: hugging-face-text-generation-inference-usage
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Usage\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"prompt_tokens\": {\n      \"type\": \"integer\"\n    },\n    \"completion_tokens\": {\n      \"type\": \"integer\"\n    },\n    \"total_tokens\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-text-generation-inference-usage-schema.json
tags: []
title: Usage
---
