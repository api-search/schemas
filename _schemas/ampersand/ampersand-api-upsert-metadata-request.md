---
description: Request payload for upserting metadata (fields only)
layout: schema
name: UpsertMetadataRequest
properties_list:
- description: The ID that your app uses to identify the group of users for this request.
  name: groupRef
  type: string
- description: Maps object names to field definitions
  name: fields
  type: object
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-upsert-metadata-request-schema.json
slug: ampersand-api-upsert-metadata-request
source_filename: ampersand-api-upsert-metadata-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-upsert-metadata-request-schema.json\",\n  \"title\": \"UpsertMetadataRequest\",\n  \"description\": \"Request payload for upserting metadata (fields only)\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"groupRef\": {\n      \"type\": \"string\",\n      \"description\": \"The ID that your app uses to identify the group of users for this request.\",\n      \"example\": \"group-123\"\n    },\n    \"fields\": {\n      \"type\": \"object\",\n      \"description\": \"Maps object names to field definitions\",\n      \"additionalProperties\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"$ref\": \"#/components/schemas/FieldDefinition\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"groupRef\",\n    \"fields\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-upsert-metadata-request-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: UpsertMetadataRequest
---
