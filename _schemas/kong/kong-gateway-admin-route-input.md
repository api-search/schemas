---
description: Input schema for creating or updating a Route.
layout: schema
name: RouteInput
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: protocols
  type: array
- description: ''
  name: methods
  type: array
- description: ''
  name: hosts
  type: array
- description: ''
  name: paths
  type: array
- description: ''
  name: headers
  type: object
- description: ''
  name: snis
  type: array
- description: ''
  name: sources
  type: array
- description: ''
  name: destinations
  type: array
- description: ''
  name: https_redirect_status_code
  type: integer
- description: ''
  name: regex_priority
  type: integer
- description: ''
  name: strip_path
  type: boolean
- description: ''
  name: path_handling
  type: string
- description: ''
  name: preserve_host
  type: boolean
- description: ''
  name: request_buffering
  type: boolean
- description: ''
  name: response_buffering
  type: boolean
- description: ''
  name: tags
  type: array
- description: ''
  name: service
  type: object
- description: ''
  name: expression
  type: string
- description: ''
  name: priority
  type: integer
provider_name: Kong
provider_slug: kong
schema_file: json-schema/kong-gateway-admin-route-input-schema.json
slug: kong-gateway-admin-route-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RouteInput\",\n  \"type\": \"object\",\n  \"description\": \"Input schema for creating or updating a Route.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"protocols\": {\n      \"type\": \"array\"\n    },\n    \"methods\": {\n      \"type\": \"array\"\n    },\n    \"hosts\": {\n      \"type\": \"array\"\n    },\n    \"paths\": {\n      \"type\": \"array\"\n    },\n    \"headers\": {\n      \"type\": \"object\"\n    },\n    \"snis\": {\n      \"type\": \"array\"\n    },\n    \"sources\": {\n      \"type\": \"array\"\n    },\n    \"destinations\": {\n      \"type\": \"array\"\n    },\n    \"https_redirect_status_code\": {\n      \"type\": \"integer\"\n    },\n    \"regex_priority\": {\n      \"type\": \"integer\"\n    },\n    \"strip_path\": {\n      \"type\": \"boolean\"\n    },\n    \"path_handling\": {\n      \"type\": \"string\"\n    },\n    \"preserve_host\"\
  : {\n      \"type\": \"boolean\"\n    },\n    \"request_buffering\": {\n      \"type\": \"boolean\"\n    },\n    \"response_buffering\": {\n      \"type\": \"boolean\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    },\n    \"service\": {\n      \"type\": \"object\"\n    },\n    \"expression\": {\n      \"type\": \"string\"\n    },\n    \"priority\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/json-schema/kong-gateway-admin-route-input-schema.json
tags:
- API Gateway
- Lua
- NGINX
- Open Source
title: RouteInput
---
