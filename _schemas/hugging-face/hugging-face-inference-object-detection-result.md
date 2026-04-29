---
description: ''
layout: schema
name: ObjectDetectionResult
properties_list:
- description: Detected object label
  name: label
  type: string
- description: Detection confidence score
  name: score
  type: number
- description: ''
  name: box
  type: object
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-inference-object-detection-result-schema.json
slug: hugging-face-inference-object-detection-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ObjectDetectionResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Detected object label\"\n    },\n    \"score\": {\n      \"type\": \"number\",\n      \"description\": \"Detection confidence score\"\n    },\n    \"box\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-inference-object-detection-result-schema.json
tags: []
title: ObjectDetectionResult
---
