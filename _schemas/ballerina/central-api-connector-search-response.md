---
description: ConnectorSearchResponse schema from Ballerina Central API
layout: schema
name: ConnectorSearchResponse
properties_list:
- description: ''
  name: connectors
  type: array
- description: ''
  name: count
  type: integer
- description: ''
  name: offset
  type: integer
- description: ''
  name: limit
  type: integer
provider_name: Ballerina
provider_slug: ballerina
schema_file: json-schema/central-api-connector-search-response-schema.json
slug: central-api-connector-search-response
source_filename: central-api-connector-search-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/json-schema/central-api-connector-search-response-schema.json\",\n  \"title\": \"ConnectorSearchResponse\",\n  \"description\": \"ConnectorSearchResponse schema from Ballerina Central API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ConnectorSummary\"\n      }\n    },\n    \"count\": {\n      \"type\": \"integer\"\n    },\n    \"offset\": {\n      \"type\": \"integer\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/json-schema/central-api-connector-search-response-schema.json
tags:
- Integrations
- Orchestrations
- Open Source
- Programming Language
title: ConnectorSearchResponse
---
