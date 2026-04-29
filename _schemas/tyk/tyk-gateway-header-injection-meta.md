---
description: ''
layout: schema
name: HeaderInjectionMeta
properties_list:
- description: ''
  name: act_on
  type: boolean
- description: ''
  name: add_headers
  type: object
- description: ''
  name: delete_headers
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
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-header-injection-meta-schema.json
slug: tyk-gateway-header-injection-meta
source_filename: tyk-gateway-header-injection-meta-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HeaderInjectionMeta\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"act_on\": {\n      \"type\": \"boolean\"\n    },\n    \"add_headers\": {\n      \"type\": \"object\"\n    },\n    \"delete_headers\": {\n      \"type\": \"array\"\n    },\n    \"disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"method\": {\n      \"type\": \"string\"\n    },\n    \"path\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-header-injection-meta-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: HeaderInjectionMeta
---
