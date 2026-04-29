---
description: ''
layout: schema
name: Provider
properties_list:
- description: ''
  name: vendor
  type: string
- description: ''
  name: region
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: accelerators
  type: array
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-inference-endpoints-provider-schema.json
slug: hugging-face-inference-endpoints-provider
source_filename: hugging-face-inference-endpoints-provider-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Provider\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vendor\": {\n      \"type\": \"string\"\n    },\n    \"region\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"accelerators\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-inference-endpoints-provider-schema.json
tags: []
title: Provider
---
