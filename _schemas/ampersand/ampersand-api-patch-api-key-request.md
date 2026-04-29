---
description: PatchApiKeyRequest schema from Ampersand API
layout: schema
name: PatchApiKeyRequest
properties_list:
- description: 'Array of field paths specifying which fields to update. Allowed values include: - active - label - scopes'
  name: updateMask
  type: array
- description: ''
  name: apiKey
  type: object
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-patch-api-key-request-schema.json
slug: ampersand-api-patch-api-key-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-patch-api-key-request-schema.json\",\n  \"title\": \"PatchApiKeyRequest\",\n  \"description\": \"PatchApiKeyRequest schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"updateMask\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Array of field paths specifying which fields to update. Allowed values include:\\n- active\\n- label\\n- scopes\\n\",\n      \"example\": [\n        \"active\",\n        \"label\"\n      ]\n    },\n    \"apiKey\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"label\": {\n          \"type\": \"string\",\n          \"description\": \"A short name for the API key.\",\n          \"example\": \"MailMonkey API Key\"\n        },\n        \"active\": {\n     \
  \     \"type\": \"boolean\",\n          \"description\": \"Whether the API key is active.\",\n          \"example\": true\n        },\n        \"scopes\": {\n          \"$ref\": \"#/components/schemas/ApiKeyScopes\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"updateMask\",\n    \"apiKey\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-patch-api-key-request-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: PatchApiKeyRequest
---
