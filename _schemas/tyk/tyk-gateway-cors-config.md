---
description: ''
layout: schema
name: CORSConfig
properties_list:
- description: ''
  name: allow_credentials
  type: boolean
- description: ''
  name: allowed_headers
  type: array
- description: ''
  name: allowed_methods
  type: array
- description: ''
  name: allowed_origins
  type: array
- description: ''
  name: debug
  type: boolean
- description: ''
  name: enable
  type: boolean
- description: ''
  name: exposed_headers
  type: array
- description: ''
  name: max_age
  type: integer
- description: ''
  name: options_passthrough
  type: boolean
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-cors-config-schema.json
slug: tyk-gateway-cors-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CORSConfig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allow_credentials\": {\n      \"type\": \"boolean\"\n    },\n    \"allowed_headers\": {\n      \"type\": \"array\"\n    },\n    \"allowed_methods\": {\n      \"type\": \"array\"\n    },\n    \"allowed_origins\": {\n      \"type\": \"array\"\n    },\n    \"debug\": {\n      \"type\": \"boolean\"\n    },\n    \"enable\": {\n      \"type\": \"boolean\"\n    },\n    \"exposed_headers\": {\n      \"type\": \"array\"\n    },\n    \"max_age\": {\n      \"type\": \"integer\"\n    },\n    \"options_passthrough\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-cors-config-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: CORSConfig
---
