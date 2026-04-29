---
description: PropertyGraphStreamRecord schema from Neptune
layout: schema
name: PropertyGraphStreamRecord
properties_list:
- description: Unix epoch timestamp in milliseconds of the transaction commit.
  name: commitTimestamp
  type: integer
- description: ''
  name: eventId
  type: object
- description: ''
  name: data
  type: object
- description: The operation type (ADD or REMOVE).
  name: op
  type: string
- description: True only if this is the last operation in the transaction.
  name: isLastOp
  type: boolean
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/streams-property-graph-stream-record-schema.json
slug: streams-property-graph-stream-record
source_filename: streams-property-graph-stream-record-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/streams-property-graph-stream-record-schema.json\",\n  \"title\": \"PropertyGraphStreamRecord\",\n  \"description\": \"PropertyGraphStreamRecord schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"commitTimestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix epoch timestamp in milliseconds of the transaction commit.\"\n    },\n    \"eventId\": {\n      \"$ref\": \"#/components/schemas/StreamEventId\"\n    },\n    \"data\": {\n      \"$ref\": \"#/components/schemas/PropertyGraphData\"\n    },\n    \"op\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ADD\",\n        \"REMOVE\"\n      ],\n      \"description\": \"The operation type (ADD or REMOVE).\"\n    },\n    \"isLastOp\": {\n      \"type\": \"boolean\",\n      \"description\": \"True only if\
  \ this is the last operation in the transaction.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/streams-property-graph-stream-record-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: PropertyGraphStreamRecord
---
