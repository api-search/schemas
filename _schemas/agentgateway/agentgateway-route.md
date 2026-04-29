---
description: A routing rule in AgentGateway that matches incoming requests and forwards them to a backend or MCP target.
layout: schema
name: Route
properties_list:
- description: Unique name for this route.
  name: name
  type: string
- description: List of matching criteria for this route.
  name: matches
  type: array
- description: Name of the LLM backend to forward matched requests to.
  name: backend
  type: string
- description: Rate limiting configuration for this route.
  name: rateLimit
  type: object
- description: Retry policy for failed requests.
  name: retries
  type: object
provider_name: AgentGateway
provider_slug: agentgateway
schema_file: json-schema/agentgateway-route-schema.json
slug: agentgateway-route
source_filename: agentgateway-route-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agentgateway/refs/heads/main/json-schema/agentgateway-route-schema.json\",\n  \"title\": \"Route\",\n  \"description\": \"A routing rule in AgentGateway that matches incoming requests and forwards them to a backend or MCP target.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name for this route.\",\n      \"example\": \"openai-route\"\n    },\n    \"matches\": {\n      \"type\": \"array\",\n      \"description\": \"List of matching criteria for this route.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"headers\": {\n            \"type\": \"array\",\n            \"description\": \"Header-based match criteria.\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n           \
  \     \"name\": { \"type\": \"string\" },\n                \"value\": { \"type\": \"string\" }\n              }\n            }\n          },\n          \"path\": {\n            \"type\": \"object\",\n            \"description\": \"Path-based match criteria.\",\n            \"properties\": {\n              \"prefix\": { \"type\": \"string\" },\n              \"exact\": { \"type\": \"string\" }\n            }\n          }\n        }\n      }\n    },\n    \"backend\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the LLM backend to forward matched requests to.\",\n      \"example\": \"openai-gpt4\"\n    },\n    \"rateLimit\": {\n      \"type\": \"object\",\n      \"description\": \"Rate limiting configuration for this route.\",\n      \"properties\": {\n        \"requestsPerSecond\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum requests per second.\",\n          \"example\": 10\n        },\n        \"burstSize\": {\n          \"type\": \"integer\"\
  ,\n          \"description\": \"Maximum burst size above the rate limit.\",\n          \"example\": 20\n        }\n      }\n    },\n    \"retries\": {\n      \"type\": \"object\",\n      \"description\": \"Retry policy for failed requests.\",\n      \"properties\": {\n        \"attempts\": { \"type\": \"integer\", \"example\": 3 },\n        \"perTryTimeout\": { \"type\": \"string\", \"example\": \"30s\" }\n      }\n    }\n  },\n  \"required\": [\"name\", \"backend\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agentgateway/refs/heads/main/json-schema/agentgateway-route-schema.json
tags:
- AI Gateway
- API Gateway
- MCP
- LLM
- Agent-to-Agent
- Open Source
- CNCF
- Observability
- Security
title: Route
---
