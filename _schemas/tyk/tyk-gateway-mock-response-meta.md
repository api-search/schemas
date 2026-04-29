---
description: ''
layout: schema
name: MockResponseMeta
properties_list:
- description: ''
  name: body
  type: string
- description: ''
  name: code
  type: integer
- description: ''
  name: disabled
  type: boolean
- description: ''
  name: headers
  type: object
- description: ''
  name: ignore_case
  type: boolean
- description: ''
  name: method
  type: string
- description: ''
  name: path
  type: string
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-mock-response-meta-schema.json
slug: tyk-gateway-mock-response-meta
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MockResponseMeta\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"body\": {\n      \"type\": \"string\"\n    },\n    \"code\": {\n      \"type\": \"integer\"\n    },\n    \"disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"headers\": {\n      \"type\": \"object\"\n    },\n    \"ignore_case\": {\n      \"type\": \"boolean\"\n    },\n    \"method\": {\n      \"type\": \"string\"\n    },\n    \"path\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-mock-response-meta-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: MockResponseMeta
---
