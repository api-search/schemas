---
description: ''
layout: schema
name: RateLimitMeta
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
  name: per
  type: number
- description: ''
  name: rate
  type: number
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-rate-limit-meta-schema.json
slug: tyk-gateway-rate-limit-meta
source_filename: tyk-gateway-rate-limit-meta-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RateLimitMeta\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"method\": {\n      \"type\": \"string\"\n    },\n    \"path\": {\n      \"type\": \"string\"\n    },\n    \"per\": {\n      \"type\": \"number\"\n    },\n    \"rate\": {\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-rate-limit-meta-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: RateLimitMeta
---
