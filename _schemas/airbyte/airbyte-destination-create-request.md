---
description: DestinationCreateRequest schema from Airbyte API
layout: schema
name: DestinationCreateRequest
properties_list:
- description: Name of the destination e.g. dev-mysql-instance.
  name: name
  type: string
- description: The UUID of the connector definition. One of configuration.destinationType or definitionId must be provided.
  name: definitionId
  type: string
- description: ''
  name: workspaceId
  type: string
- description: ''
  name: configuration
  type: object
- description: ''
  name: resourceAllocation
  type: object
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-destination-create-request-schema.json
slug: airbyte-destination-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-destination-create-request-schema.json\",\n  \"title\": \"DestinationCreateRequest\",\n  \"description\": \"DestinationCreateRequest schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"Name of the destination e.g. dev-mysql-instance.\",\n      \"type\": \"string\"\n    },\n    \"definitionId\": {\n      \"description\": \"The UUID of the connector definition. One of configuration.destinationType or definitionId must be provided.\",\n      \"format\": \"uuid\",\n      \"type\": \"string\"\n    },\n    \"workspaceId\": {\n      \"format\": \"uuid\",\n      \"type\": \"string\"\n    },\n    \"configuration\": {\n      \"$ref\": \"#/components/schemas/DestinationConfiguration\"\n    },\n    \"resourceAllocation\": {\n      \"$ref\": \"#/components/schemas/ScopedResourceRequirements\"\
  \n    }\n  },\n  \"required\": [\n    \"name\",\n    \"workspaceId\",\n    \"configuration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-destination-create-request-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: DestinationCreateRequest
---
