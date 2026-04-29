---
description: ''
layout: schema
name: TextClassificationRequest
properties_list:
- description: The text to classify
  name: inputs
  type: string
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-inference-text-classification-request-schema.json
slug: hugging-face-inference-text-classification-request
source_filename: hugging-face-inference-text-classification-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TextClassificationRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"string\",\n      \"description\": \"The text to classify\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-inference-text-classification-request-schema.json
tags: []
title: TextClassificationRequest
---
