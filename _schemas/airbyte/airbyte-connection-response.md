---
description: Provides details of a single connection.
layout: schema
name: ConnectionResponse
properties_list:
- description: ''
  name: connectionId
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: sourceId
  type: string
- description: ''
  name: destinationId
  type: string
- description: ''
  name: workspaceId
  type: string
- description: ''
  name: status
  type: object
- description: ''
  name: schedule
  type: object
- description: ''
  name: nonBreakingSchemaUpdatesBehavior
  type: object
- description: ''
  name: namespaceDefinition
  type: object
- description: ''
  name: namespaceFormat
  type: string
- description: ''
  name: prefix
  type: string
- description: ''
  name: configurations
  type: object
- description: ''
  name: createdAt
  type: integer
- description: ''
  name: tags
  type: array
- description: ''
  name: statusReason
  type: string
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-connection-response-schema.json
slug: airbyte-connection-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-connection-response-schema.json\",\n  \"title\": \"ConnectionResponse\",\n  \"description\": \"Provides details of a single connection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectionId\": {\n      \"format\": \"UUID\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"sourceId\": {\n      \"format\": \"UUID\",\n      \"type\": \"string\"\n    },\n    \"destinationId\": {\n      \"format\": \"UUID\",\n      \"type\": \"string\"\n    },\n    \"workspaceId\": {\n      \"format\": \"UUID\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"$ref\": \"#/components/schemas/ConnectionStatusEnum\"\n    },\n    \"schedule\": {\n      \"$ref\": \"#/components/schemas/ConnectionScheduleResponse\"\n    },\n    \"nonBreakingSchemaUpdatesBehavior\"\
  : {\n      \"$ref\": \"#/components/schemas/NonBreakingSchemaUpdatesBehaviorEnum\"\n    },\n    \"namespaceDefinition\": {\n      \"$ref\": \"#/components/schemas/NamespaceDefinitionEnum\"\n    },\n    \"namespaceFormat\": {\n      \"type\": \"string\"\n    },\n    \"prefix\": {\n      \"type\": \"string\"\n    },\n    \"configurations\": {\n      \"$ref\": \"#/components/schemas/StreamConfigurations\"\n    },\n    \"createdAt\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Tag\"\n      }\n    },\n    \"statusReason\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"connectionId\",\n    \"name\",\n    \"sourceId\",\n    \"destinationId\",\n    \"workspaceId\",\n    \"status\",\n    \"schedule\",\n    \"configurations\",\n    \"createdAt\",\n    \"tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-connection-response-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: ConnectionResponse
---
