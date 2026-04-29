---
description: ''
layout: schema
name: AuthConfig
properties_list:
- description: ''
  name: auth_header_name
  type: string
- description: ''
  name: cookie_name
  type: string
- description: ''
  name: disable_header
  type: boolean
- description: ''
  name: name
  type: string
- description: ''
  name: param_name
  type: string
- description: ''
  name: use_certificate
  type: boolean
- description: ''
  name: use_cookie
  type: boolean
- description: ''
  name: use_param
  type: boolean
- description: ''
  name: validate_signature
  type: boolean
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-auth-config-schema.json
slug: tyk-gateway-auth-config
source_filename: tyk-gateway-auth-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AuthConfig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"auth_header_name\": {\n      \"type\": \"string\"\n    },\n    \"cookie_name\": {\n      \"type\": \"string\"\n    },\n    \"disable_header\": {\n      \"type\": \"boolean\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"param_name\": {\n      \"type\": \"string\"\n    },\n    \"use_certificate\": {\n      \"type\": \"boolean\"\n    },\n    \"use_cookie\": {\n      \"type\": \"boolean\"\n    },\n    \"use_param\": {\n      \"type\": \"boolean\"\n    },\n    \"validate_signature\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-auth-config-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: AuthConfig
---
