---
description: ''
layout: schema
name: URLRewrite
properties_list:
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: pattern
  type: string
- description: ''
  name: rewriteTo
  type: string
- description: ''
  name: triggers
  type: array
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-url-rewrite-schema.json
slug: tyk-gateway-url-rewrite
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"URLRewrite\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"pattern\": {\n      \"type\": \"string\"\n    },\n    \"rewriteTo\": {\n      \"type\": \"string\"\n    },\n    \"triggers\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-url-rewrite-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: URLRewrite
---
