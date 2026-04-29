---
description: ''
layout: schema
name: ZeroShotClassificationResponse
properties_list:
- description: ''
  name: sequence
  type: string
- description: ''
  name: labels
  type: array
- description: ''
  name: scores
  type: array
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-inference-zero-shot-classification-response-schema.json
slug: hugging-face-inference-zero-shot-classification-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ZeroShotClassificationResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sequence\": {\n      \"type\": \"string\"\n    },\n    \"labels\": {\n      \"type\": \"array\"\n    },\n    \"scores\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-inference-zero-shot-classification-response-schema.json
tags: []
title: ZeroShotClassificationResponse
---
