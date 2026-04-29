---
description: ''
layout: schema
name: GenerateRequest
properties_list:
- description: Input prompt text
  name: inputs
  type: string
- description: ''
  name: parameters
  type: object
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-text-generation-inference-generate-request-schema.json
slug: hugging-face-text-generation-inference-generate-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GenerateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"string\",\n      \"description\": \"Input prompt text\"\n    },\n    \"parameters\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-text-generation-inference-generate-request-schema.json
tags: []
title: GenerateRequest
---
