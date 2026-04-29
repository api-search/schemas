---
description: ''
layout: schema
name: SourcesResponse
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
schema_file: json-schema/airbyte-sources-response-schema.json
slug: airbyte-sources-response
source_filename: airbyte-sources-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-sources-response-schema.json\",\n  \"title\": \"SourcesResponse\",\n  \"description\": \"\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"previous\": {\n      \"type\": \"string\"\n    },\n    \"next\": {\n      \"type\": \"string\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SourceResponse\"\n      }\n    }\n  },\n  \"required\": [\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-sources-response-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: SourcesResponse
---
