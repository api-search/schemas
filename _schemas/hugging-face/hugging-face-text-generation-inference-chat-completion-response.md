---
description: ''
layout: schema
name: ChatCompletionResponse
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: object
  type: string
- description: ''
  name: created
  type: integer
- description: ''
  name: model
  type: string
- description: ''
  name: system_fingerprint
  type: string
- description: ''
  name: choices
  type: array
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-text-generation-inference-chat-completion-response-schema.json
slug: hugging-face-text-generation-inference-chat-completion-response
source_filename: hugging-face-text-generation-inference-chat-completion-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChatCompletionResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"object\": {\n      \"type\": \"string\"\n    },\n    \"created\": {\n      \"type\": \"integer\"\n    },\n    \"model\": {\n      \"type\": \"string\"\n    },\n    \"system_fingerprint\": {\n      \"type\": \"string\"\n    },\n    \"choices\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-text-generation-inference-chat-completion-response-schema.json
tags: []
title: ChatCompletionResponse
---
