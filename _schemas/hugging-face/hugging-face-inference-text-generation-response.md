---
description: ''
layout: schema
name: TextGenerationResponse
properties_list:
- description: The generated text
  name: generated_text
  type: string
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-inference-text-generation-response-schema.json
slug: hugging-face-inference-text-generation-response
source_filename: hugging-face-inference-text-generation-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TextGenerationResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"generated_text\": {\n      \"type\": \"string\",\n      \"description\": \"The generated text\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-inference-text-generation-response-schema.json
tags: []
title: TextGenerationResponse
---
