---
description: ''
layout: schema
name: VirtualMeta
properties_list:
- description: ''
  name: disabled
  type: boolean
- description: ''
  name: function_source_type
  type: string
- description: ''
  name: function_source_uri
  type: string
- description: ''
  name: method
  type: string
- description: ''
  name: path
  type: string
- description: ''
  name: proxy_on_error
  type: boolean
- description: ''
  name: response_function_name
  type: string
- description: ''
  name: use_session
  type: boolean
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-virtual-meta-schema.json
slug: tyk-gateway-virtual-meta
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VirtualMeta\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"function_source_type\": {\n      \"type\": \"string\"\n    },\n    \"function_source_uri\": {\n      \"type\": \"string\"\n    },\n    \"method\": {\n      \"type\": \"string\"\n    },\n    \"path\": {\n      \"type\": \"string\"\n    },\n    \"proxy_on_error\": {\n      \"type\": \"boolean\"\n    },\n    \"response_function_name\": {\n      \"type\": \"string\"\n    },\n    \"use_session\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-virtual-meta-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: VirtualMeta
---
