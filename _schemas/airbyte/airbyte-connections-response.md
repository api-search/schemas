---
description: ''
layout: schema
name: ConnectionsResponse
properties_list:
- description: ''
  name: previous
  type: string
- description: ''
  name: next
  type: string
- description: ''
  name: data
  type: array
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-connections-response-schema.json
slug: airbyte-connections-response
source_filename: airbyte-connections-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-connections-response-schema.json\",\n  \"title\": \"ConnectionsResponse\",\n  \"description\": \"\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"previous\": {\n      \"type\": \"string\"\n    },\n    \"next\": {\n      \"type\": \"string\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ConnectionResponse\"\n      },\n      \"default\": []\n    }\n  },\n  \"required\": [\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-connections-response-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: ConnectionsResponse
---
