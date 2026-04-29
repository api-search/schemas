---
description: ''
layout: schema
name: GatewayInput
properties_list:
- description: The name of the gateway.
  name: name
  type: string
- description: Enable response caching.
  name: cache_enabled
  type: boolean
- description: Cache TTL in seconds.
  name: cache_ttl
  type: integer
- description: Enable rate limiting.
  name: rate_limiting_enabled
  type: boolean
- description: Rate limit threshold.
  name: rate_limiting_limit
  type: integer
- description: Rate limiting interval in seconds.
  name: rate_limiting_interval
  type: integer
- description: Enable request logging.
  name: log_enabled
  type: boolean
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-ai-gateway-gateway-input-schema.json
slug: cloudflare-ai-gateway-gateway-input
source_filename: cloudflare-ai-gateway-gateway-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GatewayInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the gateway.\"\n    },\n    \"cache_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enable response caching.\"\n    },\n    \"cache_ttl\": {\n      \"type\": \"integer\",\n      \"description\": \"Cache TTL in seconds.\"\n    },\n    \"rate_limiting_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enable rate limiting.\"\n    },\n    \"rate_limiting_limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Rate limit threshold.\"\n    },\n    \"rate_limiting_interval\": {\n      \"type\": \"integer\",\n      \"description\": \"Rate limiting interval in seconds.\"\n    },\n    \"log_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enable request logging.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-ai-gateway-gateway-input-schema.json
tags:
- AI Gateway
- API Gateway
- Artificial Intelligence
- CDN
- Cloud
- Containers
- DDoS Protection
- DNS
- Edge
- Edge Computing
- Object Storage
- Platform
- Real-Time Communication
- Security
- Serverless
- Web Performance
title: GatewayInput
---
