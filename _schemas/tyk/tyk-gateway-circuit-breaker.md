---
description: ''
layout: schema
name: CircuitBreaker
properties_list:
- description: ''
  name: coolDownPeriod
  type: integer
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: halfOpenStateEnabled
  type: boolean
- description: ''
  name: sampleSize
  type: integer
- description: ''
  name: threshold
  type: number
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-circuit-breaker-schema.json
slug: tyk-gateway-circuit-breaker
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CircuitBreaker\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"coolDownPeriod\": {\n      \"type\": \"integer\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"halfOpenStateEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"sampleSize\": {\n      \"type\": \"integer\"\n    },\n    \"threshold\": {\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-circuit-breaker-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: CircuitBreaker
---
