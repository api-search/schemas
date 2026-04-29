---
description: ''
layout: schema
name: UpstreamInput
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: algorithm
  type: string
- description: ''
  name: hash_on
  type: string
- description: ''
  name: hash_fallback
  type: string
- description: ''
  name: hash_on_header
  type: string
- description: ''
  name: hash_fallback_header
  type: string
- description: ''
  name: hash_on_cookie
  type: string
- description: ''
  name: hash_on_cookie_path
  type: string
- description: ''
  name: hash_on_query_arg
  type: string
- description: ''
  name: hash_fallback_query_arg
  type: string
- description: ''
  name: hash_on_uri_capture
  type: string
- description: ''
  name: hash_fallback_uri_capture
  type: string
- description: ''
  name: slots
  type: integer
- description: ''
  name: tags
  type: array
- description: ''
  name: host_header
  type: string
- description: ''
  name: use_srv_name
  type: boolean
provider_name: Kong
provider_slug: kong
schema_file: json-schema/kong-gateway-admin-upstream-input-schema.json
slug: kong-gateway-admin-upstream-input
source_filename: kong-gateway-admin-upstream-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpstreamInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"algorithm\": {\n      \"type\": \"string\"\n    },\n    \"hash_on\": {\n      \"type\": \"string\"\n    },\n    \"hash_fallback\": {\n      \"type\": \"string\"\n    },\n    \"hash_on_header\": {\n      \"type\": \"string\"\n    },\n    \"hash_fallback_header\": {\n      \"type\": \"string\"\n    },\n    \"hash_on_cookie\": {\n      \"type\": \"string\"\n    },\n    \"hash_on_cookie_path\": {\n      \"type\": \"string\"\n    },\n    \"hash_on_query_arg\": {\n      \"type\": \"string\"\n    },\n    \"hash_fallback_query_arg\": {\n      \"type\": \"string\"\n    },\n    \"hash_on_uri_capture\": {\n      \"type\": \"string\"\n    },\n    \"hash_fallback_uri_capture\": {\n      \"type\": \"string\"\n    },\n    \"slots\": {\n      \"type\": \"integer\"\n    },\n    \"tags\"\
  : {\n      \"type\": \"array\"\n    },\n    \"host_header\": {\n      \"type\": \"string\"\n    },\n    \"use_srv_name\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/json-schema/kong-gateway-admin-upstream-input-schema.json
tags:
- API Gateway
- Lua
- NGINX
- Open Source
title: UpstreamInput
---
