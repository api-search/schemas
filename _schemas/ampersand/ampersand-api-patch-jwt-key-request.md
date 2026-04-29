---
description: PatchJWTKeyRequest schema from Ampersand API
layout: schema
name: PatchJWTKeyRequest
properties_list:
- description: List of field paths to update (currently supports 'active' and 'name')
  name: updateMask
  type: array
- description: Object containing the fields to update with their new values
  name: jwtKey
  type: object
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-patch-jwt-key-request-schema.json
slug: ampersand-api-patch-jwt-key-request
source_filename: ampersand-api-patch-jwt-key-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-patch-jwt-key-request-schema.json\",\n  \"title\": \"PatchJWTKeyRequest\",\n  \"description\": \"PatchJWTKeyRequest schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"updateMask\": {\n      \"type\": \"array\",\n      \"description\": \"List of field paths to update (currently supports 'active' and 'name')\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"active\",\n          \"label\"\n        ]\n      },\n      \"minItems\": 1,\n      \"example\": [\n        \"active\",\n        \"label\"\n      ]\n    },\n    \"jwtKey\": {\n      \"type\": \"object\",\n      \"description\": \"Object containing the fields to update with their new values\",\n      \"additionalProperties\": true,\n      \"properties\": {\n        \"active\":\
  \ {\n          \"type\": \"boolean\",\n          \"description\": \"New active status for the JWT key\",\n          \"example\": false\n        },\n        \"label\": {\n          \"type\": \"string\",\n          \"description\": \"New label for the JWT key\",\n          \"example\": \"updated-key-name\"\n        }\n      },\n      \"example\": {\n        \"active\": false,\n        \"name\": \"updated-key-name\"\n      }\n    }\n  },\n  \"required\": [\n    \"updateMask\",\n    \"jwtKey\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-patch-jwt-key-request-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: PatchJWTKeyRequest
---
