---
description: ''
layout: schema
name: ErrorResponse
properties_list:
- description: Error message
  name: error
  type: string
- description: Error type classification
  name: error_type
  type: string
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-text-generation-inference-error-response-schema.json
slug: hugging-face-text-generation-inference-error-response
source_filename: hugging-face-text-generation-inference-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Error message\"\n    },\n    \"error_type\": {\n      \"type\": \"string\",\n      \"description\": \"Error type classification\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-text-generation-inference-error-response-schema.json
tags: []
title: ErrorResponse
---
