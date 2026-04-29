---
description: Provides details of a single connector definition.
layout: schema
name: ConnectorDefinitionResponse
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: connectorDefinitionType
  type: object
- description: ''
  name: version
  type: string
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-connector-definition-response-schema.json
slug: airbyte-connector-definition-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-connector-definition-response-schema.json\",\n  \"title\": \"ConnectorDefinitionResponse\",\n  \"description\": \"Provides details of a single connector definition.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"format\": \"UUID\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"connectorDefinitionType\": {\n      \"$ref\": \"#/components/schemas/ConnectorType\"\n    },\n    \"version\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"connectorDefinitionType\",\n    \"name\",\n    \"version\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-connector-definition-response-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: ConnectorDefinitionResponse
---
