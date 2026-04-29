---
description: ''
layout: schema
name: ValidatePathMeta
properties_list:
- description: ''
  name: disabled
  type: boolean
- description: ''
  name: error_response_code
  type: integer
- description: ''
  name: method
  type: string
- description: ''
  name: path
  type: string
- description: ''
  name: schema
  type: object
- description: ''
  name: schema_b64
  type: string
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-validate-path-meta-schema.json
slug: tyk-gateway-validate-path-meta
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ValidatePathMeta\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"error_response_code\": {\n      \"type\": \"integer\"\n    },\n    \"method\": {\n      \"type\": \"string\"\n    },\n    \"path\": {\n      \"type\": \"string\"\n    },\n    \"schema\": {\n      \"type\": \"object\"\n    },\n    \"schema_b64\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-validate-path-meta-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: ValidatePathMeta
---
