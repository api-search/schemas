---
description: ''
layout: schema
name: CachePlugin
properties_list:
- description: ''
  name: cacheByRegex
  type: string
- description: ''
  name: cacheResponseCodes
  type: array
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: timeout
  type: integer
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-cache-plugin-schema.json
slug: tyk-gateway-cache-plugin
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CachePlugin\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cacheByRegex\": {\n      \"type\": \"string\"\n    },\n    \"cacheResponseCodes\": {\n      \"type\": \"array\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"timeout\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-cache-plugin-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: CachePlugin
---
