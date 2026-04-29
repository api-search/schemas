---
description: ''
layout: schema
name: GlobalRateLimit
properties_list:
- description: ''
  name: disabled
  type: boolean
- description: ''
  name: per
  type: number
- description: ''
  name: rate
  type: number
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-global-rate-limit-schema.json
slug: tyk-gateway-global-rate-limit
source_filename: tyk-gateway-global-rate-limit-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GlobalRateLimit\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"per\": {\n      \"type\": \"number\"\n    },\n    \"rate\": {\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-global-rate-limit-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: GlobalRateLimit
---
