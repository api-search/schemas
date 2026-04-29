---
description: CreateDefinitionRequest schema from Airbyte API
layout: schema
name: CreateDefinitionRequest
properties_list:
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
schema_file: json-schema/airbyte-create-definition-request-schema.json
slug: airbyte-create-definition-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-create-definition-request-schema.json\",\n  \"title\": \"CreateDefinitionRequest\",\n  \"description\": \"CreateDefinitionRequest schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"dockerRepository\": {\n      \"type\": \"string\"\n    },\n    \"dockerImageTag\": {\n      \"type\": \"string\"\n    },\n    \"documentationUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"dockerRepository\",\n    \"dockerImageTag\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-create-definition-request-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: CreateDefinitionRequest
---
