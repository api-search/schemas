---
description: Cross-Origin Resource Sharing configuration
layout: schema
name: CORSPolicy
properties_list:
- description: Allowed origins. Use a string for exact match or a regex pattern.
  name: origins
  type: array
- description: Allowed HTTP methods
  name: methods
  type: array
- description: Allowed request headers
  name: headers
  type: array
- description: Whether to allow credentials (cookies, authorization headers)
  name: credentials
  type: boolean
- description: Headers exposed to the browser
  name: exposed_headers
  type: array
- description: How long the preflight response can be cached (e.g., '86400')
  name: max_age
  type: string
provider_name: Ambassador
provider_slug: ambassador
schema_file: json-schema/ambassador-cors-policy-schema.json
slug: ambassador-cors-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CORSPolicy\",\n  \"type\": \"object\",\n  \"description\": \"Cross-Origin Resource Sharing configuration\",\n  \"properties\": {\n    \"origins\": {\n      \"type\": \"array\",\n      \"description\": \"Allowed origins. Use a string for exact match or a regex pattern.\"\n    },\n    \"methods\": {\n      \"type\": \"array\",\n      \"description\": \"Allowed HTTP methods\"\n    },\n    \"headers\": {\n      \"type\": \"array\",\n      \"description\": \"Allowed request headers\"\n    },\n    \"credentials\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to allow credentials (cookies, authorization headers)\"\n    },\n    \"exposed_headers\": {\n      \"type\": \"array\",\n      \"description\": \"Headers exposed to the browser\"\n    },\n    \"max_age\": {\n      \"type\": \"string\",\n      \"description\": \"How long the preflight response can be cached (e.g., '86400')\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/json-schema/ambassador-cors-policy-schema.json
tags:
- API Development
- Gateways
- Ingress
- Kubernetes
- Mock Servers
- Mocks
- Platform
- Testing
title: CORSPolicy
---
