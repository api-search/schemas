---
description: ''
layout: schema
name: ModelLoadingResponse
properties_list:
- description: Error message indicating the model is loading
  name: error
  type: string
- description: Estimated time in seconds until the model is ready
  name: estimated_time
  type: number
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-inference-model-loading-response-schema.json
slug: hugging-face-inference-model-loading-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ModelLoadingResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Error message indicating the model is loading\"\n    },\n    \"estimated_time\": {\n      \"type\": \"number\",\n      \"description\": \"Estimated time in seconds until the model is ready\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-inference-model-loading-response-schema.json
tags: []
title: ModelLoadingResponse
---
