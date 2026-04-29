---
description: ''
layout: schema
name: CompletionRequest
properties_list:
- description: Model ID to use
  name: model
  type: string
- description: Prompt(s) to generate completions for
  name: prompt
  type: string
- description: ''
  name: max_tokens
  type: integer
- description: ''
  name: temperature
  type: number
- description: ''
  name: top_p
  type: number
- description: ''
  name: stop
  type: array
- description: ''
  name: stream
  type: boolean
- description: ''
  name: seed
  type: integer
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-inference-providers-completion-request-schema.json
slug: hugging-face-inference-providers-completion-request
source_filename: hugging-face-inference-providers-completion-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompletionRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Model ID to use\"\n    },\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"Prompt(s) to generate completions for\"\n    },\n    \"max_tokens\": {\n      \"type\": \"integer\"\n    },\n    \"temperature\": {\n      \"type\": \"number\"\n    },\n    \"top_p\": {\n      \"type\": \"number\"\n    },\n    \"stop\": {\n      \"type\": \"array\"\n    },\n    \"stream\": {\n      \"type\": \"boolean\"\n    },\n    \"seed\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-inference-providers-completion-request-schema.json
tags: []
title: CompletionRequest
---
