---
description: ApiKeyRequest schema from Ampersand API
layout: schema
name: ApiKeyRequest
properties_list:
- description: A short name for the API key.
  name: label
  type: string
- description: ''
  name: scopes
  type: object
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-api-key-request-schema.json
slug: ampersand-api-api-key-request
source_filename: ampersand-api-api-key-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-api-key-request-schema.json\",\n  \"title\": \"ApiKeyRequest\",\n  \"description\": \"ApiKeyRequest schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"A short name for the API key.\",\n      \"example\": \"MailMonkey API Key\"\n    },\n    \"scopes\": {\n      \"$ref\": \"#/components/schemas/ApiKeyScopes\"\n    }\n  },\n  \"required\": [\n    \"label\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-api-key-request-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: ApiKeyRequest
---
