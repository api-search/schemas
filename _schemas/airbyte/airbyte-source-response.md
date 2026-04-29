---
description: Provides details of a single source.
layout: schema
name: SourceResponse
properties_list:
- description: ''
  name: sourceId
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: sourceType
  type: string
- description: ''
  name: definitionId
  type: string
- description: ''
  name: workspaceId
  type: string
- description: ''
  name: configuration
  type: object
- description: ''
  name: createdAt
  type: integer
- description: ''
  name: resourceAllocation
  type: object
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-source-response-schema.json
slug: airbyte-source-response
source_filename: airbyte-source-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-source-response-schema.json\",\n  \"title\": \"SourceResponse\",\n  \"description\": \"Provides details of a single source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourceId\": {\n      \"format\": \"UUID\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"sourceType\": {\n      \"type\": \"string\"\n    },\n    \"definitionId\": {\n      \"format\": \"UUID\",\n      \"type\": \"string\"\n    },\n    \"workspaceId\": {\n      \"format\": \"UUID\",\n      \"type\": \"string\"\n    },\n    \"configuration\": {\n      \"$ref\": \"#/components/schemas/SourceConfiguration\"\n    },\n    \"createdAt\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"resourceAllocation\": {\n      \"$ref\": \"#/components/schemas/ScopedResourceRequirements\"\
  \n    }\n  },\n  \"required\": [\n    \"sourceId\",\n    \"name\",\n    \"sourceType\",\n    \"workspaceId\",\n    \"configuration\",\n    \"definitionId\",\n    \"createdAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-source-response-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: SourceResponse
---
