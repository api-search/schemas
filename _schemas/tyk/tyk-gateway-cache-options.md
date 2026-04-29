---
description: ''
layout: schema
name: CacheOptions
properties_list:
- description: ''
  name: cache_all_safe_requests
  type: boolean
- description: ''
  name: cache_by_headers
  type: array
- description: ''
  name: cache_control_ttl_header
  type: string
- description: ''
  name: cache_response_codes
  type: array
- description: ''
  name: cache_timeout
  type: integer
- description: ''
  name: enable_cache
  type: boolean
- description: ''
  name: enable_upstream_cache_control
  type: boolean
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-cache-options-schema.json
slug: tyk-gateway-cache-options
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CacheOptions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cache_all_safe_requests\": {\n      \"type\": \"boolean\"\n    },\n    \"cache_by_headers\": {\n      \"type\": \"array\"\n    },\n    \"cache_control_ttl_header\": {\n      \"type\": \"string\"\n    },\n    \"cache_response_codes\": {\n      \"type\": \"array\"\n    },\n    \"cache_timeout\": {\n      \"type\": \"integer\"\n    },\n    \"enable_cache\": {\n      \"type\": \"boolean\"\n    },\n    \"enable_upstream_cache_control\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-cache-options-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: CacheOptions
---
