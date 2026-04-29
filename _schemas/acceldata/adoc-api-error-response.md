---
description: Error response
layout: schema
name: ErrorResponse
properties_list:
- description: Human-readable error message
  name: message
  type: string
- description: Error code
  name: error
  type: string
- description: HTTP-style error code
  name: code
  type: integer
provider_name: Acceldata
provider_slug: acceldata
schema_file: json-schema/adoc-api-error-response-schema.json
slug: adoc-api-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://acceldata.io/schemas/error-response.json\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"description\": \"Error response\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message\"\n    },\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Error code\"\n    },\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP-style error code\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/json-schema/adoc-api-error-response-schema.json
tags:
- AI Agents
- Data Management
- Data Observability
- Data Pipeline
- Data Quality
- Intelligence
- Observability
title: ErrorResponse
---
