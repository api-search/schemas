---
description: ''
layout: schema
name: ErrorResponse
properties_list:
- description: Error message
  name: message
  type: string
- description: Error code
  name: code
  type: integer
provider_name: ArchiMate
provider_slug: archimate
schema_file: json-schema/archimate-model-exchange-api-error-response-schema.json
slug: archimate-model-exchange-api-error-response
source_filename: archimate-model-exchange-api-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Error message\",\n      \"example\": \"Unauthorized\"\n    },\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"Error code\",\n      \"example\": 401\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archimate/refs/heads/main/json-schema/archimate-model-exchange-api-error-response-schema.json\",\n  \"title\": \"ErrorResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archimate/refs/heads/main/json-schema/archimate-model-exchange-api-error-response-schema.json
tags:
- Enterprise Architecture
- Architecture Framework
- Modeling Language
- Business Architecture
- Technology Architecture
- Standard
- Open Group
title: ErrorResponse
---
