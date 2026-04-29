---
description: ''
layout: schema
name: CacheMeta
properties_list:
- description: ''
  name: cache_key_regex
  type: string
- description: ''
  name: cache_response_codes
  type: array
- description: ''
  name: disabled
  type: boolean
- description: ''
  name: method
  type: string
- description: ''
  name: path
  type: string
- description: ''
  name: timeout
  type: integer
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-cache-meta-schema.json
slug: tyk-gateway-cache-meta
source_filename: tyk-gateway-cache-meta-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CacheMeta\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cache_key_regex\": {\n      \"type\": \"string\"\n    },\n    \"cache_response_codes\": {\n      \"type\": \"array\"\n    },\n    \"disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"method\": {\n      \"type\": \"string\"\n    },\n    \"path\": {\n      \"type\": \"string\"\n    },\n    \"timeout\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-cache-meta-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: CacheMeta
---
