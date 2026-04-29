---
description: An Ambassador RateLimit resource that defines rate limiting policies using descriptors and rate values. Works with the built-in Ambassador Edge Stack rate limiting service.
layout: schema
name: RateLimit
properties_list:
- description: ''
  name: apiVersion
  type: string
- description: ''
  name: kind
  type: string
provider_name: Ambassador
provider_slug: ambassador
schema_file: json-schema/ambassador-rate-limit-schema.json
slug: ambassador-rate-limit
source_filename: ambassador-rate-limit-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RateLimit\",\n  \"type\": \"object\",\n  \"description\": \"An Ambassador RateLimit resource that defines rate limiting policies using descriptors and rate values. Works with the built-in Ambassador Edge Stack rate limiting service.\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/json-schema/ambassador-rate-limit-schema.json
tags:
- API Development
- Gateways
- Ingress
- Kubernetes
- Mock Servers
- Mocks
- Platform
- Testing
title: RateLimit
---
