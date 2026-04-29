---
description: ''
layout: schema
name: InferenceRequest
properties_list:
- description: The input data for inference
  name: inputs
  type: string
- description: Task-specific parameters
  name: parameters
  type: object
- description: ''
  name: options
  type: object
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-inference-inference-request-schema.json
slug: hugging-face-inference-inference-request
source_filename: hugging-face-inference-inference-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InferenceRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"string\",\n      \"description\": \"The input data for inference\"\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"description\": \"Task-specific parameters\"\n    },\n    \"options\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-inference-inference-request-schema.json
tags: []
title: InferenceRequest
---
