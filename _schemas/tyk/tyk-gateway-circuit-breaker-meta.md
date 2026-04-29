---
description: ''
layout: schema
name: CircuitBreakerMeta
properties_list:
- description: ''
  name: disable_half_open_state
  type: boolean
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
  name: return_to_service_after
  type: integer
- description: ''
  name: samples
  type: integer
- description: ''
  name: threshold_percent
  type: number
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-circuit-breaker-meta-schema.json
slug: tyk-gateway-circuit-breaker-meta
source_filename: tyk-gateway-circuit-breaker-meta-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CircuitBreakerMeta\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"disable_half_open_state\": {\n      \"type\": \"boolean\"\n    },\n    \"disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"method\": {\n      \"type\": \"string\"\n    },\n    \"path\": {\n      \"type\": \"string\"\n    },\n    \"return_to_service_after\": {\n      \"type\": \"integer\"\n    },\n    \"samples\": {\n      \"type\": \"integer\"\n    },\n    \"threshold_percent\": {\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-circuit-breaker-meta-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: CircuitBreakerMeta
---
