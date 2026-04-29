---
description: List of RateLimit resources
layout: schema
name: RateLimitList
properties_list:
- description: ''
  name: apiVersion
  type: string
- description: ''
  name: kind
  type: string
- description: ''
  name: metadata
  type: object
- description: ''
  name: items
  type: array
provider_name: Ambassador
provider_slug: ambassador
schema_file: json-schema/ambassador-rate-limit-list-schema.json
slug: ambassador-rate-limit-list
source_filename: ambassador-rate-limit-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RateLimitList\",\n  \"type\": \"object\",\n  \"description\": \"List of RateLimit resources\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    },\n    \"metadata\": {\n      \"type\": \"object\"\n    },\n    \"items\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/json-schema/ambassador-rate-limit-list-schema.json
tags:
- API Development
- Gateways
- Ingress
- Kubernetes
- Mock Servers
- Mocks
- Platform
- Testing
title: RateLimitList
---
