---
description: ErrorResponse from Adobe API
layout: schema
name: ErrorResponse
properties_list:
- description: Machine-readable error code.
  name: error_code
  type: string
- description: Human-readable error description.
  name: message
  type: string
provider_name: Adobe Creative Cloud
provider_slug: adobe-creative-cloud
schema_file: json-schema/adobe-firefly-api-error-response-schema.json
slug: adobe-firefly-api-error-response
source_filename: adobe-firefly-api-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-firefly-api-error-response-schema.json\",\n  \"title\": \"ErrorResponse\",\n  \"description\": \"ErrorResponse from Adobe API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error_code\": {\n      \"type\": \"string\",\n      \"description\": \"Machine-readable error code.\",\n      \"example\": \"example_value\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error description.\",\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-firefly-api-error-response-schema.json
tags:
- AI/ML
- Cloud
- Creative
- Design
- Documents
- Photography
- SaaS
- Video
title: ErrorResponse
---
