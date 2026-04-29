---
description: ''
layout: schema
name: URLRewriteMeta
properties_list:
- description: ''
  name: disabled
  type: boolean
- description: ''
  name: match_pattern
  type: string
- description: ''
  name: method
  type: string
- description: ''
  name: path
  type: string
- description: ''
  name: rewrite_to
  type: string
- description: ''
  name: triggers
  type: array
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-url-rewrite-meta-schema.json
slug: tyk-gateway-url-rewrite-meta
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"URLRewriteMeta\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"match_pattern\": {\n      \"type\": \"string\"\n    },\n    \"method\": {\n      \"type\": \"string\"\n    },\n    \"path\": {\n      \"type\": \"string\"\n    },\n    \"rewrite_to\": {\n      \"type\": \"string\"\n    },\n    \"triggers\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-url-rewrite-meta-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: URLRewriteMeta
---
