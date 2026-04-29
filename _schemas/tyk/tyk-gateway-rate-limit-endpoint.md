---
description: ''
layout: schema
name: RateLimitEndpoint
properties_list:
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: per
  type: integer
- description: ''
  name: rate
  type: integer
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-rate-limit-endpoint-schema.json
slug: tyk-gateway-rate-limit-endpoint
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RateLimitEndpoint\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"per\": {\n      \"type\": \"integer\"\n    },\n    \"rate\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-rate-limit-endpoint-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: RateLimitEndpoint
---
