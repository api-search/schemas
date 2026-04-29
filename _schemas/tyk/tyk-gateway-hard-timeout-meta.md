---
description: ''
layout: schema
name: HardTimeoutMeta
properties_list:
- description: ''
  name: disabled
  type: boolean
- description: ''
  name: method
  type: string
- description: ''
  name: path
  type: string
- description: ''
  name: timeout
  type: integer
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-hard-timeout-meta-schema.json
slug: tyk-gateway-hard-timeout-meta
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HardTimeoutMeta\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"method\": {\n      \"type\": \"string\"\n    },\n    \"path\": {\n      \"type\": \"string\"\n    },\n    \"timeout\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-hard-timeout-meta-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: HardTimeoutMeta
---
