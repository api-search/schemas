---
description: Standard error response from the iControl REST API.
layout: schema
name: ErrorResponse
properties_list:
- description: HTTP status code.
  name: code
  type: integer
- description: Error message describing what went wrong.
  name: message
  type: string
- description: Stack trace for debugging (when available).
  name: errorStack
  type: array
- description: API-specific error code.
  name: apiError
  type: integer
provider_name: F5 Networks
provider_slug: f5-networks
schema_file: json-schema/bigip-icontrol-rest-error-response-schema.json
slug: bigip-icontrol-rest-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"description\": \"Standard error response from the iControl REST API.\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP status code.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Error message describing what went wrong.\"\n    },\n    \"errorStack\": {\n      \"type\": \"array\",\n      \"description\": \"Stack trace for debugging (when available).\"\n    },\n    \"apiError\": {\n      \"type\": \"integer\",\n      \"description\": \"API-specific error code.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/f5-networks/refs/heads/main/json-schema/bigip-icontrol-rest-error-response-schema.json
tags:
- API Gateway
- Application Delivery
- Automation
- Edge Computing
- Kubernetes
- Load Balancing
- Multi-Cloud
- NGINX
- Security
- WAF
title: ErrorResponse
---
