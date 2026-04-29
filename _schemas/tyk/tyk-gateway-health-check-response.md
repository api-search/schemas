---
description: ''
layout: schema
name: HealthCheckResponse
properties_list:
- description: ''
  name: description
  type: string
- description: ''
  name: details
  type: object
- description: ''
  name: output
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: version
  type: string
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-health-check-response-schema.json
slug: tyk-gateway-health-check-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HealthCheckResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"details\": {\n      \"type\": \"object\"\n    },\n    \"output\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-health-check-response-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: HealthCheckResponse
---
