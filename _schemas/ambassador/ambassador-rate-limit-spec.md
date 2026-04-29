---
description: Specification for a RateLimit resource
layout: schema
name: RateLimitSpec
properties_list:
- description: Rate limiting domain that groups related rate limit configurations. Typically set to 'ambassador'.
  name: domain
  type: string
- description: List of rate limit rules
  name: limits
  type: array
provider_name: Ambassador
provider_slug: ambassador
schema_file: json-schema/ambassador-rate-limit-spec-schema.json
slug: ambassador-rate-limit-spec
source_filename: ambassador-rate-limit-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RateLimitSpec\",\n  \"type\": \"object\",\n  \"description\": \"Specification for a RateLimit resource\",\n  \"properties\": {\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"Rate limiting domain that groups related rate limit configurations. Typically set to 'ambassador'.\"\n    },\n    \"limits\": {\n      \"type\": \"array\",\n      \"description\": \"List of rate limit rules\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/json-schema/ambassador-rate-limit-spec-schema.json
tags:
- API Development
- Gateways
- Ingress
- Kubernetes
- Mock Servers
- Mocks
- Platform
- Testing
title: RateLimitSpec
---
