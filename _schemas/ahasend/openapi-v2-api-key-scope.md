---
description: APIKeyScope schema from AhaSend API
layout: schema
name: APIKeyScope
properties_list:
- description: Unique identifier for the scope
  name: id
  type: string
- description: When the scope was created
  name: created_at
  type: string
- description: When the scope was last updated
  name: updated_at
  type: string
- description: ID of the API key this scope belongs to
  name: api_key_id
  type: string
- description: The scope string
  name: scope
  type: string
- description: Domain ID for domain-specific scopes
  name: domain_id
  type: string
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-api-key-scope-schema.json
slug: openapi-v2-api-key-scope
source_filename: openapi-v2-api-key-scope-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-api-key-scope-schema.json\",\n  \"title\": \"APIKeyScope\",\n  \"description\": \"APIKeyScope schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the scope\",\n      \"example\": \"500123\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the scope was created\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the scope was last updated\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"api_key_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\
  ,\n      \"description\": \"ID of the API key this scope belongs to\",\n      \"example\": \"500123\"\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"description\": \"The scope string\",\n      \"example\": \"example_value\"\n    },\n    \"domain_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Domain ID for domain-specific scopes\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"created_at\",\n    \"updated_at\",\n    \"api_key_id\",\n    \"scope\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-api-key-scope-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: APIKeyScope
---
