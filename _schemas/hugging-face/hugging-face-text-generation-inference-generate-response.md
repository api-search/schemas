---
description: ''
layout: schema
name: GenerateResponse
properties_list:
- description: The generated text
  name: generated_text
  type: string
- description: ''
  name: details
  type: object
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-text-generation-inference-generate-response-schema.json
slug: hugging-face-text-generation-inference-generate-response
source_filename: hugging-face-text-generation-inference-generate-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GenerateResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"generated_text\": {\n      \"type\": \"string\",\n      \"description\": \"The generated text\"\n    },\n    \"details\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-text-generation-inference-generate-response-schema.json
tags: []
title: GenerateResponse
---
