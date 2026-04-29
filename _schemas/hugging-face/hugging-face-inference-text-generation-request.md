---
description: ''
layout: schema
name: TextGenerationRequest
properties_list:
- description: The prompt text to generate from
  name: inputs
  type: string
- description: ''
  name: parameters
  type: object
- description: ''
  name: options
  type: object
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-inference-text-generation-request-schema.json
slug: hugging-face-inference-text-generation-request
source_filename: hugging-face-inference-text-generation-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TextGenerationRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"string\",\n      \"description\": \"The prompt text to generate from\"\n    },\n    \"parameters\": {\n      \"type\": \"object\"\n    },\n    \"options\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-inference-text-generation-request-schema.json
tags: []
title: TextGenerationRequest
---
