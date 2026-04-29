---
description: ''
layout: schema
name: Gateway
properties_list:
- description: The unique identifier of the gateway.
  name: id
  type: string
- description: The name of the gateway.
  name: name
  type: string
- description: URL-friendly slug for the gateway.
  name: slug
  type: string
- description: Whether response caching is enabled.
  name: cache_enabled
  type: boolean
- description: Cache time-to-live in seconds.
  name: cache_ttl
  type: integer
- description: Whether rate limiting is enabled.
  name: rate_limiting_enabled
  type: boolean
- description: Maximum requests per rate limiting interval.
  name: rate_limiting_limit
  type: integer
- description: Rate limiting interval in seconds.
  name: rate_limiting_interval
  type: integer
- description: Whether logging is enabled.
  name: log_enabled
  type: boolean
- description: When the gateway was created.
  name: created_at
  type: string
- description: When the gateway was last modified.
  name: modified_at
  type: string
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-ai-gateway-gateway-schema.json
slug: cloudflare-ai-gateway-gateway
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Gateway\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the gateway.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the gateway.\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"URL-friendly slug for the gateway.\"\n    },\n    \"cache_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether response caching is enabled.\"\n    },\n    \"cache_ttl\": {\n      \"type\": \"integer\",\n      \"description\": \"Cache time-to-live in seconds.\"\n    },\n    \"rate_limiting_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether rate limiting is enabled.\"\n    },\n    \"rate_limiting_limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum requests per rate limiting\
  \ interval.\"\n    },\n    \"rate_limiting_interval\": {\n      \"type\": \"integer\",\n      \"description\": \"Rate limiting interval in seconds.\"\n    },\n    \"log_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether logging is enabled.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the gateway was created.\"\n    },\n    \"modified_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the gateway was last modified.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-ai-gateway-gateway-schema.json
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
title: Gateway
---
