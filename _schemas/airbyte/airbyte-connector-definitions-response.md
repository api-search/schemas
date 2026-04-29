---
description: ''
layout: schema
name: ConnectorDefinitionsResponse
properties_list:
- description: ''
  name: data
  type: array
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-connector-definitions-response-schema.json
slug: airbyte-connector-definitions-response
source_filename: airbyte-connector-definitions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-connector-definitions-response-schema.json\",\n  \"title\": \"ConnectorDefinitionsResponse\",\n  \"description\": \"\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ConnectorDefinitionResponse\"\n      }\n    }\n  },\n  \"required\": [\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-connector-definitions-response-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: ConnectorDefinitionsResponse
---
