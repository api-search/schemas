---
description: ''
layout: schema
name: Model
properties_list:
- description: The identifier of the model.
  name: id
  type: string
- description: The name of the model.
  name: name
  type: string
- description: The description of the model.
  name: description
  type: string
- description: The schema for the model. For application/json models, this should be JSON schema draft 4 model.
  name: schema
  type: string
- description: The content type for the model.
  name: contentType
  type: string
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-model-schema.json
slug: amazon-api-gateway-model
source_filename: amazon-api-gateway-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Model\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the model.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the model.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the model.\"\n    },\n    \"schema\": {\n      \"type\": \"string\",\n      \"description\": \"The schema for the model. For application/json models, this should be JSON schema draft 4 model.\"\n    },\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"The content type for the model.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-model-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: Model
---
