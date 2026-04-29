---
description: ''
layout: schema
name: Endpoint
properties_list:
- description: Endpoint name
  name: name
  type: string
- description: Endpoint type
  name: type
  type: string
- description: ''
  name: accountId
  type: string
- description: ''
  name: provider
  type: object
- description: ''
  name: compute
  type: object
- description: ''
  name: model
  type: object
- description: ''
  name: status
  type: object
- description: Inference URL for the endpoint
  name: url
  type: string
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-inference-endpoints-endpoint-schema.json
slug: hugging-face-inference-endpoints-endpoint
source_filename: hugging-face-inference-endpoints-endpoint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Endpoint\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Endpoint name\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Endpoint type\"\n    },\n    \"accountId\": {\n      \"type\": \"string\"\n    },\n    \"provider\": {\n      \"type\": \"object\"\n    },\n    \"compute\": {\n      \"type\": \"object\"\n    },\n    \"model\": {\n      \"type\": \"object\"\n    },\n    \"status\": {\n      \"type\": \"object\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"Inference URL for the endpoint\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-inference-endpoints-endpoint-schema.json
tags: []
title: Endpoint
---
