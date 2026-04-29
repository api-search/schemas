---
description: ''
layout: schema
name: CORS
properties_list:
- description: ''
  name: allowCredentials
  type: boolean
- description: ''
  name: allowedHeaders
  type: array
- description: ''
  name: allowedMethods
  type: array
- description: ''
  name: allowedOrigins
  type: array
- description: ''
  name: debug
  type: boolean
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: exposedHeaders
  type: array
- description: ''
  name: maxAge
  type: integer
- description: ''
  name: optionsPassthrough
  type: boolean
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-cors-schema.json
slug: tyk-gateway-cors
source_filename: tyk-gateway-cors-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CORS\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowCredentials\": {\n      \"type\": \"boolean\"\n    },\n    \"allowedHeaders\": {\n      \"type\": \"array\"\n    },\n    \"allowedMethods\": {\n      \"type\": \"array\"\n    },\n    \"allowedOrigins\": {\n      \"type\": \"array\"\n    },\n    \"debug\": {\n      \"type\": \"boolean\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"exposedHeaders\": {\n      \"type\": \"array\"\n    },\n    \"maxAge\": {\n      \"type\": \"integer\"\n    },\n    \"optionsPassthrough\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-cors-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: CORS
---
