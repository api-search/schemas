---
description: ''
layout: schema
name: HMAC
properties_list:
- description: ''
  name: allowedAlgorithms
  type: array
- description: ''
  name: allowedClockSkew
  type: number
- description: ''
  name: enabled
  type: boolean
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-hmac-schema.json
slug: tyk-gateway-hmac
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HMAC\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowedAlgorithms\": {\n      \"type\": \"array\"\n    },\n    \"allowedClockSkew\": {\n      \"type\": \"number\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-hmac-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: HMAC
---
