---
description: ''
layout: schema
name: EndPointMeta
properties_list:
- description: ''
  name: disabled
  type: boolean
- description: ''
  name: ignore_case
  type: boolean
- description: ''
  name: method
  type: string
- description: ''
  name: method_actions
  type: object
- description: ''
  name: path
  type: string
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-end-point-meta-schema.json
slug: tyk-gateway-end-point-meta
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EndPointMeta\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"ignore_case\": {\n      \"type\": \"boolean\"\n    },\n    \"method\": {\n      \"type\": \"string\"\n    },\n    \"method_actions\": {\n      \"type\": \"object\"\n    },\n    \"path\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-end-point-meta-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: EndPointMeta
---
