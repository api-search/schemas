---
description: PropertyGraphStreamResponse schema from Neptune
layout: schema
name: PropertyGraphStreamResponse
properties_list:
- description: ''
  name: lastEventId
  type: object
- description: Unix epoch timestamp in milliseconds of the last commit.
  name: lastTrxTimestamp
  type: integer
- description: The serialization format (always PG_JSON for property graph).
  name: format
  type: string
- description: The array of change-log stream records.
  name: records
  type: array
- description: Total number of records in the response.
  name: totalRecords
  type: integer
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/streams-property-graph-stream-response-schema.json
slug: streams-property-graph-stream-response
source_filename: streams-property-graph-stream-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/streams-property-graph-stream-response-schema.json\",\n  \"title\": \"PropertyGraphStreamResponse\",\n  \"description\": \"PropertyGraphStreamResponse schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lastEventId\": {\n      \"$ref\": \"#/components/schemas/StreamEventId\"\n    },\n    \"lastTrxTimestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix epoch timestamp in milliseconds of the last commit.\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PG_JSON\"\n      ],\n      \"description\": \"The serialization format (always PG_JSON for property graph).\"\n    },\n    \"records\": {\n      \"type\": \"array\",\n      \"description\": \"The array of change-log stream records.\",\n      \"items\": {\n        \"$ref\": \"\
  #/components/schemas/PropertyGraphStreamRecord\"\n      }\n    },\n    \"totalRecords\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of records in the response.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/streams-property-graph-stream-response-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: PropertyGraphStreamResponse
---
