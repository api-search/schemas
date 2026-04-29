---
description: ''
layout: schema
name: StreamResponse
properties_list:
- description: ''
  name: token
  type: object
- description: Full generated text (only in the last event)
  name: generated_text
  type: string
- description: Generation details (only in the last event)
  name: details
  type: object
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-text-generation-inference-stream-response-schema.json
slug: hugging-face-text-generation-inference-stream-response
source_filename: hugging-face-text-generation-inference-stream-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StreamResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"object\"\n    },\n    \"generated_text\": {\n      \"type\": \"string\",\n      \"description\": \"Full generated text (only in the last event)\"\n    },\n    \"details\": {\n      \"type\": \"object\",\n      \"description\": \"Generation details (only in the last event)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-text-generation-inference-stream-response-schema.json
tags: []
title: StreamResponse
---
