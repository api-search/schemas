---
description: Standard error response from the Figma API.
layout: schema
name: ErrorResponse
properties_list:
- description: Always true for error responses.
  name: error
  type: boolean
- description: The HTTP status code.
  name: status
  type: integer
- description: A human-readable description of the error.
  name: message
  type: string
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-rest-error-response-schema.json
slug: figma-rest-error-response
source_filename: figma-rest-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"description\": \"Standard error response from the Figma API.\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"boolean\",\n      \"description\": \"Always true for error responses.\"\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"The HTTP status code.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the error.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-rest-error-response-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: ErrorResponse
---
