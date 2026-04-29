---
description: HydratedRevision schema from Ampersand API
layout: schema
name: HydratedRevision
properties_list:
- description: The revision ID.
  name: id
  type: string
- description: The spec version string.
  name: specVersion
  type: string
- description: The time the revision was created.
  name: createTime
  type: string
- description: ''
  name: content
  type: object
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-hydrated-revision-schema.json
slug: ampersand-api-hydrated-revision
source_filename: ampersand-api-hydrated-revision-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-hydrated-revision-schema.json\",\n  \"title\": \"HydratedRevision\",\n  \"description\": \"HydratedRevision schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The revision ID.\",\n      \"example\": \"f0e1d2c3-b4a5-6789-0abc-def123456789\"\n    },\n    \"specVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The spec version string.\",\n      \"example\": \"1.0.0\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the revision was created.\",\n      \"format\": \"date-time\"\n    },\n    \"content\": {\n      \"$ref\": \"../manifest/manifest.yaml#/components/schemas/HydratedIntegration\"\n    }\n  },\n  \"required\": [\n    \"content\",\n  \
  \  \"createTime\",\n    \"id\",\n    \"specVersion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-hydrated-revision-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: HydratedRevision
---
