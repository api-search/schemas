---
description: ObjectMetadata schema from Ampersand API
layout: schema
name: ObjectMetadata
properties_list:
- description: The provider name of the object
  name: name
  type: string
- description: Human-readable name of the object
  name: displayName
  type: string
- description: The mapped name of the object as defined in your integration config, if a mapping was applied. Only present when using the installation-scoped metadata endpoint.
  name: mappedObjectName
  type: string
- description: Map of field metadata keyed by field name
  name: fields
  type: object
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-object-metadata-schema.json
slug: ampersand-api-object-metadata
source_filename: ampersand-api-object-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-object-metadata-schema.json\",\n  \"title\": \"ObjectMetadata\",\n  \"description\": \"ObjectMetadata schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The provider name of the object\",\n      \"example\": \"contact\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the object\",\n      \"example\": \"Contact\"\n    },\n    \"mappedObjectName\": {\n      \"type\": \"string\",\n      \"description\": \"The mapped name of the object as defined in your integration config, if a mapping was applied. Only present when using the installation-scoped metadata endpoint.\",\n      \"example\": \"people\"\n    },\n    \"fields\": {\n      \"type\": \"\
  object\",\n      \"description\": \"Map of field metadata keyed by field name\",\n      \"additionalProperties\": {\n        \"$ref\": \"../manifest/manifest.yaml#/components/schemas/FieldMetadata\"\n      }\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"fields\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-object-metadata-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: ObjectMetadata
---
