---
description: Represents an API endpoint discovered by the Lunar Gateway through observed traffic, including request metrics such as count, latency, and status code distributions.
layout: schema
name: Lunar.dev Discovered Endpoint
properties_list:
- description: HTTP method observed for this endpoint.
  name: method
  type: string
- description: The URL pattern of the discovered endpoint.
  name: url
  type: string
- description: Distribution of HTTP status codes observed for this endpoint.
  name: status_codes
  type: object
- description: Total number of requests observed for this endpoint.
  name: count
  type: integer
- description: Average latency in milliseconds for requests to this endpoint.
  name: average_latency_ms
  type: number
provider_name: Lunar.dev
provider_slug: lunar-dev
schema_file: json-schema/discovered-endpoint.json
slug: discovered-endpoint
source_filename: discovered-endpoint.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/lunar-dev/blob/main/json-schema/discovered-endpoint.json\",\n  \"title\": \"Lunar.dev Discovered Endpoint\",\n  \"description\": \"Represents an API endpoint discovered by the Lunar Gateway through observed traffic, including request metrics such as count, latency, and status code distributions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"method\": {\n      \"type\": \"string\",\n      \"description\": \"HTTP method observed for this endpoint.\",\n      \"examples\": [\n        \"GET\",\n        \"POST\"\n      ]\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The URL pattern of the discovered endpoint.\",\n      \"examples\": [\n        \"api.example.com/v1/users\"\n      ]\n    },\n    \"status_codes\": {\n      \"type\": \"object\",\n      \"description\": \"Distribution of HTTP status codes observed for this endpoint.\"\
  ,\n      \"additionalProperties\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of requests observed for this endpoint.\"\n    },\n    \"average_latency_ms\": {\n      \"type\": \"number\",\n      \"description\": \"Average latency in milliseconds for requests to this endpoint.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lunar-dev/refs/heads/main/json-schema/discovered-endpoint.json
tags:
- AI Gateway
- Automation
- Consumption Gateway
- Control
- Deployment
- Integrations
- MCP Gateway
- Performance
- Platform
- Version Control
- Visibility
- Workflows
title: Lunar.dev Discovered Endpoint
---
