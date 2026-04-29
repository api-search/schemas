---
description: SparqlStreamResponse schema from Neptune
layout: schema
name: SparqlStreamResponse
properties_list:
- description: ''
  name: lastEventId
  type: object
- description: Unix epoch timestamp in milliseconds of the last commit.
  name: lastTrxTimestamp
  type: integer
- description: The serialization format (always NQUADS for RDF).
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
schema_file: json-schema/streams-sparql-stream-response-schema.json
slug: streams-sparql-stream-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/streams-sparql-stream-response-schema.json\",\n  \"title\": \"SparqlStreamResponse\",\n  \"description\": \"SparqlStreamResponse schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lastEventId\": {\n      \"$ref\": \"#/components/schemas/StreamEventId\"\n    },\n    \"lastTrxTimestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix epoch timestamp in milliseconds of the last commit.\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"NQUADS\"\n      ],\n      \"description\": \"The serialization format (always NQUADS for RDF).\"\n    },\n    \"records\": {\n      \"type\": \"array\",\n      \"description\": \"The array of change-log stream records.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SparqlStreamRecord\"\
  \n      }\n    },\n    \"totalRecords\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of records in the response.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/streams-sparql-stream-response-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: SparqlStreamResponse
---
