---
description: ''
layout: schema
name: RateLimitSmoothing
properties_list:
- description: ''
  name: delay
  type: integer
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: step
  type: integer
- description: ''
  name: threshold
  type: integer
- description: ''
  name: trigger
  type: number
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-rate-limit-smoothing-schema.json
slug: tyk-gateway-rate-limit-smoothing
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RateLimitSmoothing\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"delay\": {\n      \"type\": \"integer\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"step\": {\n      \"type\": \"integer\"\n    },\n    \"threshold\": {\n      \"type\": \"integer\"\n    },\n    \"trigger\": {\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-rate-limit-smoothing-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: RateLimitSmoothing
---
