---
description: Standard error response
layout: schema
name: ErrorResponse
properties_list:
- description: Numeric error code
  name: code
  type: integer
- description: Human-readable error description
  name: message
  type: string
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-stock-error-response-schema.json
slug: adobe-creative-suite-stock-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-stock-error-response-schema.json\",\n  \"title\": \"ErrorResponse\",\n  \"description\": \"Standard error response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric error code\",\n      \"example\": 1920\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error description\",\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-stock-error-response-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: ErrorResponse
---
