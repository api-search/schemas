---
description: Error response returned when a request fails.
layout: schema
name: ErrorResponse
properties_list:
- description: The error type identifier.
  name: '@type'
  type: string
- description: The HTTP status code.
  name: statusCode
  type: integer
- description: A human-readable error message.
  name: message
  type: string
- description: A detailed description of the error.
  name: description
  type: string
- description: The unique request ID for troubleshooting.
  name: requestId
  type: string
provider_name: Informatica
provider_slug: informatica
schema_file: json-schema/informatica-platform-rest-error-response-schema.json
slug: informatica-platform-rest-error-response
source_filename: informatica-platform-rest-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"description\": \"Error response returned when a request fails.\",\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The error type identifier.\"\n    },\n    \"statusCode\": {\n      \"type\": \"integer\",\n      \"description\": \"The HTTP status code.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable error message.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A detailed description of the error.\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique request ID for troubleshooting.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/json-schema/informatica-platform-rest-error-response-schema.json
tags:
- Address Verification
- B2B Gateway
- Cloud Services
- Data Governance
- Data Integration
- Data Profiling
- Data Quality
- Enterprise Software
- ETL
- IDMC
- IICS
- Master Data Management
- Reference Data Management
title: ErrorResponse
---
