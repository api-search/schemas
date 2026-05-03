---
description: Represents a TaxiQL query submitted to the Orbital data gateway for execution against connected data sources.
layout: schema
name: Orbital Query
properties_list:
- description: Unique identifier for this query execution.
  name: queryId
  type: string
- description: The TaxiQL query string to execute.
  name: query
  type: string
- description: Controls how type metadata is included in the response.
  name: resultMode
  type: string
- description: Array of result records matching the query.
  name: results
  type: array
- description: Query execution duration in milliseconds.
  name: duration
  type: integer
provider_name: Orbital
provider_slug: orbital
schema_file: json-schema/query.json
slug: query
source_filename: query.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/orbital/refs/heads/main/json-schema/query.json\",\n  \"title\": \"Orbital Query\",\n  \"description\": \"Represents a TaxiQL query submitted to the Orbital data gateway for execution against connected data sources.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"queryId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this query execution.\"\n    },\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"The TaxiQL query string to execute.\"\n    },\n    \"resultMode\": {\n      \"type\": \"string\",\n      \"description\": \"Controls how type metadata is included in the response.\",\n      \"enum\": [\"RAW\", \"TYPED\"],\n      \"default\": \"RAW\"\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"Array of result records matching the query.\",\n      \"items\"\
  : {\n        \"type\": \"object\",\n        \"additionalProperties\": true\n      }\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Query execution duration in milliseconds.\"\n    }\n  },\n  \"required\": [\"query\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/orbital/refs/heads/main/json-schema/query.json
tags:
- Data
- Gateways
title: Orbital Query
---
