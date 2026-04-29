---
description: Provides details of a single destination.
layout: schema
name: DestinationResponse
properties_list:
- description: ''
  name: destinationId
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: destinationType
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
schema_file: json-schema/airbyte-destination-response-schema.json
slug: airbyte-destination-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-destination-response-schema.json\",\n  \"title\": \"DestinationResponse\",\n  \"description\": \"Provides details of a single destination.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"destinationId\": {\n      \"format\": \"UUID\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"destinationType\": {\n      \"type\": \"string\"\n    },\n    \"definitionId\": {\n      \"format\": \"UUID\",\n      \"type\": \"string\"\n    },\n    \"workspaceId\": {\n      \"format\": \"UUID\",\n      \"type\": \"string\"\n    },\n    \"configuration\": {\n      \"$ref\": \"#/components/schemas/DestinationConfiguration\"\n    },\n    \"createdAt\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"resourceAllocation\": {\n      \"$ref\":\
  \ \"#/components/schemas/ScopedResourceRequirements\"\n    }\n  },\n  \"required\": [\n    \"destinationId\",\n    \"name\",\n    \"destinationType\",\n    \"definitionId\",\n    \"workspaceId\",\n    \"configuration\",\n    \"createdAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-destination-response-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: DestinationResponse
---
