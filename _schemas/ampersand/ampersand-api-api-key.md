---
description: ApiKey schema from Ampersand API
layout: schema
name: ApiKey
properties_list:
- description: The API key.
  name: key
  type: string
- description: A short name for the API key.
  name: label
  type: string
- description: ''
  name: scopes
  type: object
- description: The project ID.
  name: projectId
  type: string
- description: Whether the API key is active.
  name: active
  type: boolean
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-api-key-schema.json
slug: ampersand-api-api-key
source_filename: ampersand-api-api-key-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-api-key-schema.json\",\n  \"title\": \"ApiKey\",\n  \"description\": \"ApiKey schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The API key.\",\n      \"example\": \"api-key-123\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"A short name for the API key.\",\n      \"example\": \"MailMonkey API Key\"\n    },\n    \"scopes\": {\n      \"$ref\": \"#/components/schemas/ApiKeyScopes\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"The project ID.\",\n      \"example\": \"my-project\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the API key is active.\",\n      \"example\": true\n    }\n\
  \  },\n  \"required\": [\n    \"key\",\n    \"projectId\",\n    \"label\",\n    \"scopes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-api-key-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: ApiKey
---
