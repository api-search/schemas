---
description: ''
layout: schema
name: ZeroShotClassificationRequest
properties_list:
- description: The text to classify
  name: inputs
  type: string
- description: ''
  name: parameters
  type: object
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-inference-zero-shot-classification-request-schema.json
slug: hugging-face-inference-zero-shot-classification-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ZeroShotClassificationRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"string\",\n      \"description\": \"The text to classify\"\n    },\n    \"parameters\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-inference-zero-shot-classification-request-schema.json
tags: []
title: ZeroShotClassificationRequest
---
