---
description: ''
layout: schema
name: CreateEndpointRequest
properties_list:
- description: Unique endpoint name
  name: name
  type: string
- description: Endpoint security type
  name: type
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
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-inference-endpoints-create-endpoint-request-schema.json
slug: hugging-face-inference-endpoints-create-endpoint-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateEndpointRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique endpoint name\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Endpoint security type\"\n    },\n    \"provider\": {\n      \"type\": \"object\"\n    },\n    \"compute\": {\n      \"type\": \"object\"\n    },\n    \"model\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-inference-endpoints-create-endpoint-request-schema.json
tags: []
title: CreateEndpointRequest
---
