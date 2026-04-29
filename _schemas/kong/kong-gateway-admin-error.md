---
description: Standard error response from the Admin API.
layout: schema
name: Error
properties_list:
- description: A human-readable error message.
  name: message
  type: string
- description: The error type name.
  name: name
  type: string
- description: An optional error code.
  name: code
  type: integer
- description: Field-level validation errors.
  name: fields
  type: object
provider_name: Kong
provider_slug: kong
schema_file: json-schema/kong-gateway-admin-error-schema.json
slug: kong-gateway-admin-error
source_filename: kong-gateway-admin-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"description\": \"Standard error response from the Admin API.\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable error message.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The error type name.\"\n    },\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"An optional error code.\"\n    },\n    \"fields\": {\n      \"type\": \"object\",\n      \"description\": \"Field-level validation errors.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/json-schema/kong-gateway-admin-error-schema.json
tags:
- API Gateway
- Lua
- NGINX
- Open Source
title: Error
---
