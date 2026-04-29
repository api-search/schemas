---
description: DataplaneResponse schema from Airbyte API
layout: schema
name: DataplaneResponse
properties_list:
- description: ''
  name: dataplaneId
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: regionId
  type: string
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-dataplane-response-schema.json
slug: airbyte-dataplane-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-dataplane-response-schema.json\",\n  \"title\": \"DataplaneResponse\",\n  \"description\": \"DataplaneResponse schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dataplaneId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"regionId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"dataplaneId\",\n    \"name\",\n    \"regionId\",\n    \"enabled\",\n    \"createdAt\",\n    \"updatedAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-dataplane-response-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: DataplaneResponse
---
