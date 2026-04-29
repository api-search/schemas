---
description: Provides details of a single connector definition.
layout: schema
name: DefinitionResponse
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: dockerRepository
  type: string
- description: ''
  name: dockerImageTag
  type: string
- description: ''
  name: documentationUrl
  type: string
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-definition-response-schema.json
slug: airbyte-definition-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-definition-response-schema.json\",\n  \"title\": \"DefinitionResponse\",\n  \"description\": \"Provides details of a single connector definition.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"format\": \"UUID\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"dockerRepository\": {\n      \"type\": \"string\"\n    },\n    \"dockerImageTag\": {\n      \"type\": \"string\"\n    },\n    \"documentationUrl\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"dockerRepository\",\n    \"dockerImageTag\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-definition-response-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: DefinitionResponse
---
