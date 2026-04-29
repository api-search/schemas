---
description: ''
layout: schema
name: Error
properties_list:
- description: Error message
  name: error
  type: string
- description: Underlying exception type
  name: cause_exception
  type: string
- description: Underlying exception message
  name: cause_message
  type: string
- description: Stack trace (only in development)
  name: cause_traceback
  type: array
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-dataset-viewer-error-schema.json
slug: hugging-face-dataset-viewer-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Error message\"\n    },\n    \"cause_exception\": {\n      \"type\": \"string\",\n      \"description\": \"Underlying exception type\"\n    },\n    \"cause_message\": {\n      \"type\": \"string\",\n      \"description\": \"Underlying exception message\"\n    },\n    \"cause_traceback\": {\n      \"type\": \"array\",\n      \"description\": \"Stack trace (only in development)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-dataset-viewer-error-schema.json
tags: []
title: Error
---
