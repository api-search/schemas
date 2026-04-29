---
description: CreateAPIKeyRequest schema from AhaSend API
layout: schema
name: CreateAPIKeyRequest
properties_list:
- description: Human-readable label for the API key
  name: label
  type: string
- description: Array of scope strings to grant to this API key
  name: scopes
  type: array
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-create-api-key-request-schema.json
slug: openapi-v2-create-api-key-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-create-api-key-request-schema.json\",\n  \"title\": \"CreateAPIKeyRequest\",\n  \"description\": \"CreateAPIKeyRequest schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"label\": {\n      \"type\": \"string\",\n      \"maxLength\": 255,\n      \"description\": \"Human-readable label for the API key\",\n      \"example\": \"example_value\"\n    },\n    \"scopes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"minItems\": 1,\n      \"description\": \"Array of scope strings to grant to this API key\",\n      \"example\": [\n        \"example_value\"\n      ]\n    }\n  },\n  \"required\": [\n    \"label\",\n    \"scopes\"\n  ],\n  \"example\": {\n    \"label\": \"Production API Key\",\n    \"scopes\": [\n      \"messages:send:all\"\
  ,\n      \"domains:read\"\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-create-api-key-request-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: CreateAPIKeyRequest
---
