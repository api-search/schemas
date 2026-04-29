---
description: Circuit breaker configuration for an upstream cluster
layout: schema
name: CircuitBreaker
properties_list:
- description: Envoy routing priority
  name: priority
  type: string
- description: Maximum number of connections to the upstream cluster
  name: max_connections
  type: integer
- description: Maximum number of pending requests to the upstream cluster
  name: max_pending_requests
  type: integer
- description: Maximum number of parallel requests to the upstream cluster
  name: max_requests
  type: integer
- description: Maximum number of parallel retries to the upstream cluster
  name: max_retries
  type: integer
provider_name: Ambassador
provider_slug: ambassador
schema_file: json-schema/ambassador-circuit-breaker-schema.json
slug: ambassador-circuit-breaker
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CircuitBreaker\",\n  \"type\": \"object\",\n  \"description\": \"Circuit breaker configuration for an upstream cluster\",\n  \"properties\": {\n    \"priority\": {\n      \"type\": \"string\",\n      \"description\": \"Envoy routing priority\"\n    },\n    \"max_connections\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of connections to the upstream cluster\"\n    },\n    \"max_pending_requests\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of pending requests to the upstream cluster\"\n    },\n    \"max_requests\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of parallel requests to the upstream cluster\"\n    },\n    \"max_retries\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of parallel retries to the upstream cluster\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/json-schema/ambassador-circuit-breaker-schema.json
tags:
- API Development
- Gateways
- Ingress
- Kubernetes
- Mock Servers
- Mocks
- Platform
- Testing
title: CircuitBreaker
---
