---
description: ''
layout: schema
name: CompletionRequest
properties_list:
- description: ''
  name: model
  type: string
- description: ''
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
- description: Suffix to append after generated text
  name: suffix
  type: string
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-text-generation-inference-completion-request-schema.json
slug: hugging-face-text-generation-inference-completion-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompletionRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"model\": {\n      \"type\": \"string\"\n    },\n    \"prompt\": {\n      \"type\": \"string\"\n    },\n    \"max_tokens\": {\n      \"type\": \"integer\"\n    },\n    \"temperature\": {\n      \"type\": \"number\"\n    },\n    \"top_p\": {\n      \"type\": \"number\"\n    },\n    \"stop\": {\n      \"type\": \"array\"\n    },\n    \"stream\": {\n      \"type\": \"boolean\"\n    },\n    \"seed\": {\n      \"type\": \"integer\"\n    },\n    \"suffix\": {\n      \"type\": \"string\",\n      \"description\": \"Suffix to append after generated text\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-text-generation-inference-completion-request-schema.json
tags: []
title: CompletionRequest
---
