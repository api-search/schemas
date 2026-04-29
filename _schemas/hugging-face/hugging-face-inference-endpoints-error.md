---
description: ''
layout: schema
name: Error
properties_list:
- description: Error message
  name: error
  type: string
- description: HTTP status code
  name: statusCode
  type: integer
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-inference-endpoints-error-schema.json
slug: hugging-face-inference-endpoints-error
source_filename: hugging-face-inference-endpoints-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Error message\"\n    },\n    \"statusCode\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP status code\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-inference-endpoints-error-schema.json
tags: []
title: Error
---
