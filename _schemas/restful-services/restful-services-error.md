---
description: Standard error response format for RESTful services, aligned with RFC 7807 Problem Details for HTTP APIs.
layout: schema
name: REST Error Response
properties_list:
- description: URI reference identifying the problem type (RFC 7807)
  name: type
  type: string
- description: Short, human-readable summary of the problem type
  name: title
  type: string
- description: HTTP status code (e.g., 400, 404, 422, 500)
  name: status
  type: integer
- description: Human-readable explanation specific to this occurrence
  name: detail
  type: string
- description: URI reference identifying the specific occurrence of the problem
  name: instance
  type: string
- description: Field-level validation errors
  name: errors
  type: array
provider_name: RESTful Services
provider_slug: restful-services
schema_file: json-schema/restful-services-error-schema.json
slug: restful-services-error
source_filename: restful-services-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/restful-services/schemas/rest-error\",\n  \"title\": \"REST Error Response\",\n  \"description\": \"Standard error response format for RESTful services, aligned with RFC 7807 Problem Details for HTTP APIs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URI reference identifying the problem type (RFC 7807)\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Short, human-readable summary of the problem type\"\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP status code (e.g., 400, 404, 422, 500)\"\n    },\n    \"detail\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable explanation specific to this occurrence\"\n    },\n    \"instance\": {\n      \"type\": \"string\",\n \
  \     \"format\": \"uri\",\n      \"description\": \"URI reference identifying the specific occurrence of the problem\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"Field-level validation errors\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"field\": { \"type\": \"string\" },\n          \"message\": { \"type\": \"string\" },\n          \"code\": { \"type\": \"string\" }\n        }\n      }\n    }\n  },\n  \"required\": [\"status\", \"title\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/restful-services/refs/heads/main/json-schema/restful-services-error-schema.json
tags:
- Architecture
- HTTP
- Microservices
- REST
- Web Services
title: REST Error Response
---
