---
description: ''
layout: schema
name: Usage
properties_list:
- description: Number of tokens in the prompt
  name: prompt_tokens
  type: integer
- description: Number of tokens in the completion
  name: completion_tokens
  type: integer
- description: Total tokens used
  name: total_tokens
  type: integer
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-inference-providers-usage-schema.json
slug: hugging-face-inference-providers-usage
source_filename: hugging-face-inference-providers-usage-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Usage\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"prompt_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of tokens in the prompt\"\n    },\n    \"completion_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of tokens in the completion\"\n    },\n    \"total_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"Total tokens used\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-inference-providers-usage-schema.json
tags: []
title: Usage
---
