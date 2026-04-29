---
description: Standard error response body
layout: schema
name: ErrorResponse
properties_list:
- description: Machine-readable error code
  name: code
  type: string
- description: Human-readable description of the error
  name: message
  type: string
- description: Unique identifier for the failed request, for support purposes
  name: requestId
  type: string
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-firefly-error-response-schema.json
slug: adobe-creative-suite-firefly-error-response
source_filename: adobe-creative-suite-firefly-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-firefly-error-response-schema.json\",\n  \"title\": \"ErrorResponse\",\n  \"description\": \"Standard error response body\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Machine-readable error code\",\n      \"example\": \"example_value\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the error\",\n      \"example\": \"example_value\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the failed request, for support purposes\",\n      \"example\": \"asset_abc123\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-firefly-error-response-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: ErrorResponse
---
