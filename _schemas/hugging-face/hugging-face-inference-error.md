---
description: ''
layout: schema
name: Error
properties_list:
- description: Error message
  name: error
  type: string
- description: Estimated time until availability (for loading errors)
  name: estimated_time
  type: number
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-inference-error-schema.json
slug: hugging-face-inference-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Error message\"\n    },\n    \"estimated_time\": {\n      \"type\": \"number\",\n      \"description\": \"Estimated time until availability (for loading errors)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-inference-error-schema.json
tags: []
title: Error
---
