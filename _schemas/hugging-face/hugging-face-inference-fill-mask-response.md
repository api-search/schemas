---
description: ''
layout: schema
name: FillMaskResponse
properties_list:
- description: The complete text with filled mask
  name: sequence
  type: string
- description: Confidence score for the prediction
  name: score
  type: number
- description: Token ID of the predicted word
  name: token
  type: integer
- description: The predicted word
  name: token_str
  type: string
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-inference-fill-mask-response-schema.json
slug: hugging-face-inference-fill-mask-response
source_filename: hugging-face-inference-fill-mask-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FillMaskResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sequence\": {\n      \"type\": \"string\",\n      \"description\": \"The complete text with filled mask\"\n    },\n    \"score\": {\n      \"type\": \"number\",\n      \"description\": \"Confidence score for the prediction\"\n    },\n    \"token\": {\n      \"type\": \"integer\",\n      \"description\": \"Token ID of the predicted word\"\n    },\n    \"token_str\": {\n      \"type\": \"string\",\n      \"description\": \"The predicted word\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-inference-fill-mask-response-schema.json
tags: []
title: FillMaskResponse
---
