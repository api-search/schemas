---
description: PropertygraphStreamOutput schema from Neptune
layout: schema
name: PropertygraphStreamOutput
properties_list:
- description: ''
  name: lastEventId
  type: object
- description: Timestamp of the last transaction in milliseconds.
  name: lastTrxTimestampInMillis
  type: integer
- description: ''
  name: format
  type: string
- description: ''
  name: records
  type: array
- description: ''
  name: totalRecords
  type: integer
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/data-propertygraph-stream-output-schema.json
slug: data-propertygraph-stream-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-propertygraph-stream-output-schema.json\",\n  \"title\": \"PropertygraphStreamOutput\",\n  \"description\": \"PropertygraphStreamOutput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lastEventId\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"commitNum\": {\n          \"type\": \"integer\"\n        },\n        \"opNum\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"lastTrxTimestampInMillis\": {\n      \"type\": \"integer\",\n      \"description\": \"Timestamp of the last transaction in milliseconds.\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PG_JSON\"\n      ]\n    },\n    \"records\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PropertygraphStreamRecord\"\
  \n      }\n    },\n    \"totalRecords\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-propertygraph-stream-output-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: PropertygraphStreamOutput
---
