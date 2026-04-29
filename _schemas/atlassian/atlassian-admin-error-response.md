---
description: Standard error response.
layout: schema
name: ErrorResponse
properties_list:
- description: The HTTP status code.
  name: code
  type: integer
- description: A human-readable error message.
  name: message
  type: string
- description: Detailed error information.
  name: errors
  type: array
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-admin-error-response-schema.json
slug: atlassian-admin-error-response
source_filename: atlassian-admin-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"description\": \"Standard error response.\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"The HTTP status code.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable error message.\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"Detailed error information.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-admin-error-response-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: ErrorResponse
---
