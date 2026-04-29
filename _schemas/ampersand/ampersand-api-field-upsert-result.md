---
description: Result of an upsert operation for a single field
layout: schema
name: FieldUpsertResult
properties_list:
- description: Name of the field
  name: fieldName
  type: string
- description: Action taken (create, update, none)
  name: action
  type: string
- description: Provider-specific metadata about the field
  name: metadata
  type: object
- description: Warnings that occurred during the upsert operation
  name: warnings
  type: array
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-field-upsert-result-schema.json
slug: ampersand-api-field-upsert-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-field-upsert-result-schema.json\",\n  \"title\": \"FieldUpsertResult\",\n  \"description\": \"Result of an upsert operation for a single field\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fieldName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the field\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"Action taken (create, update, none)\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Provider-specific metadata about the field\",\n      \"additionalProperties\": true\n    },\n    \"warnings\": {\n      \"type\": \"array\",\n      \"description\": \"Warnings that occurred during the upsert operation\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n\
  \    \"fieldName\",\n    \"action\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-field-upsert-result-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: FieldUpsertResult
---
