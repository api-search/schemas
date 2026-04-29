---
description: ''
layout: schema
name: ClassificationResult
properties_list:
- description: The predicted label
  name: label
  type: string
- description: Confidence score for the label
  name: score
  type: number
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-inference-classification-result-schema.json
slug: hugging-face-inference-classification-result
source_filename: hugging-face-inference-classification-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClassificationResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"The predicted label\"\n    },\n    \"score\": {\n      \"type\": \"number\",\n      \"description\": \"Confidence score for the label\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-inference-classification-result-schema.json
tags: []
title: ClassificationResult
---
