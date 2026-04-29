---
description: ''
layout: schema
name: Cache
properties_list:
- description: ''
  name: cacheAllSafeRequests
  type: boolean
- description: ''
  name: cacheByHeaders
  type: array
- description: ''
  name: cacheResponseCodes
  type: array
- description: ''
  name: controlTTLHeaderName
  type: string
- description: ''
  name: enableUpstreamCacheControl
  type: boolean
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: timeout
  type: integer
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-cache-schema.json
slug: tyk-gateway-cache
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Cache\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cacheAllSafeRequests\": {\n      \"type\": \"boolean\"\n    },\n    \"cacheByHeaders\": {\n      \"type\": \"array\"\n    },\n    \"cacheResponseCodes\": {\n      \"type\": \"array\"\n    },\n    \"controlTTLHeaderName\": {\n      \"type\": \"string\"\n    },\n    \"enableUpstreamCacheControl\": {\n      \"type\": \"boolean\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"timeout\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-cache-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: Cache
---
