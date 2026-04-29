---
description: JWTKeyResponse schema from Ampersand API
layout: schema
name: JWTKeyResponse
properties_list:
- description: The unique key identifier (key ID) for the created JWT key
  name: kid
  type: string
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-jwt-key-response-schema.json
slug: ampersand-api-jwt-key-response
source_filename: ampersand-api-jwt-key-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-jwt-key-response-schema.json\",\n  \"title\": \"JWTKeyResponse\",\n  \"description\": \"JWTKeyResponse schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique key identifier (key ID) for the created JWT key\",\n      \"example\": \"550e8400-e29b-41d4-a716-446655440000\"\n    }\n  },\n  \"required\": [\n    \"kid\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-jwt-key-response-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: JWTKeyResponse
---
