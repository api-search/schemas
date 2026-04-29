---
description: APIKey schema from AhaSend API
layout: schema
name: APIKey
properties_list:
- description: Object type identifier
  name: object
  type: string
- description: Unique identifier for the API key
  name: id
  type: string
- description: When the API key was created
  name: created_at
  type: string
- description: When the API key was last updated
  name: updated_at
  type: string
- description: When the API key was last used (updates every 5-10 minutes)
  name: last_used_at
  type: string
- description: Account ID this API key belongs to
  name: account_id
  type: string
- description: Human-readable label for the API key
  name: label
  type: string
- description: Public portion of the API key
  name: public_key
  type: string
- description: Secret key (only returned on creation)
  name: secret_key
  type: string
- description: Scopes granted to this API key
  name: scopes
  type: array
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-api-key-schema.json
slug: openapi-v2-api-key
source_filename: openapi-v2-api-key-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-api-key-schema.json\",\n  \"title\": \"APIKey\",\n  \"description\": \"APIKey schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"api_key\"\n      ],\n      \"description\": \"Object type identifier\",\n      \"example\": \"api_key\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the API key\",\n      \"example\": \"500123\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the API key was created\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"When the API key was last updated\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"last_used_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the API key was last used (updates every 5-10 minutes)\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"account_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Account ID this API key belongs to\",\n      \"example\": \"500123\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable label for the API key\",\n      \"example\": \"example_value\"\n    },\n    \"public_key\": {\n      \"type\": \"string\",\n      \"description\": \"Public portion of the API key\",\n      \"example\": \"aha-sk-aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa\"\n    },\n    \"secret_key\": {\n      \"type\": \"string\",\n      \"description\": \"Secret key (only returned on creation)\",\n   \
  \   \"example\": \"aha-sk-aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa\"\n    },\n    \"scopes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/APIKeyScope\"\n      },\n      \"description\": \"Scopes granted to this API key\",\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"created_at\": \"2025-03-15T14:30:00Z\",\n          \"updated_at\": \"2025-03-15T14:30:00Z\",\n          \"api_key_id\": \"500123\",\n          \"scope\": \"example_value\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"object\",\n    \"id\",\n    \"created_at\",\n    \"updated_at\",\n    \"account_id\",\n    \"label\",\n    \"public_key\",\n    \"scopes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-api-key-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: APIKey
---
