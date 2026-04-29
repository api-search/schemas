---
description: Retry configuration for failed requests
layout: schema
name: RetryPolicy
properties_list:
- description: Envoy retry condition. Common values include 5xx, gateway-error, connect-failure, retriable-4xx.
  name: retry_on
  type: string
- description: Maximum number of retry attempts
  name: num_retries
  type: integer
- description: Timeout per retry attempt (e.g., '3s', '500ms')
  name: per_try_timeout
  type: string
provider_name: Ambassador
provider_slug: ambassador
schema_file: json-schema/ambassador-retry-policy-schema.json
slug: ambassador-retry-policy
source_filename: ambassador-retry-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RetryPolicy\",\n  \"type\": \"object\",\n  \"description\": \"Retry configuration for failed requests\",\n  \"properties\": {\n    \"retry_on\": {\n      \"type\": \"string\",\n      \"description\": \"Envoy retry condition. Common values include 5xx, gateway-error, connect-failure, retriable-4xx.\"\n    },\n    \"num_retries\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of retry attempts\"\n    },\n    \"per_try_timeout\": {\n      \"type\": \"string\",\n      \"description\": \"Timeout per retry attempt (e.g., '3s', '500ms')\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/json-schema/ambassador-retry-policy-schema.json
tags:
- API Development
- Gateways
- Ingress
- Kubernetes
- Mock Servers
- Mocks
- Platform
- Testing
title: RetryPolicy
---
