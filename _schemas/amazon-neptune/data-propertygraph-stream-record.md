---
description: PropertygraphStreamRecord schema from Neptune
layout: schema
name: PropertygraphStreamRecord
properties_list:
- description: ''
  name: commitTimestampInMillis
  type: integer
- description: ''
  name: eventId
  type: object
- description: ''
  name: data
  type: object
- description: ''
  name: op
  type: string
- description: ''
  name: isLastOp
  type: boolean
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/data-propertygraph-stream-record-schema.json
slug: data-propertygraph-stream-record
source_filename: data-propertygraph-stream-record-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-propertygraph-stream-record-schema.json\",\n  \"title\": \"PropertygraphStreamRecord\",\n  \"description\": \"PropertygraphStreamRecord schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"commitTimestampInMillis\": {\n      \"type\": \"integer\"\n    },\n    \"eventId\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"commitNum\": {\n          \"type\": \"integer\"\n        },\n        \"opNum\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of the element (v=vertex, vl=vertex label, vp=vertex property, e=edge, ep=edge\
  \ property).\"\n        },\n        \"key\": {\n          \"type\": \"string\"\n        },\n        \"value\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"value\": {\n              \"description\": \"The property value.\"\n            },\n            \"dataType\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"from\": {\n          \"type\": \"string\",\n          \"description\": \"Source vertex ID (for edges only).\"\n        },\n        \"to\": {\n          \"type\": \"string\",\n          \"description\": \"Target vertex ID (for edges only).\"\n        }\n      }\n    },\n    \"op\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ADD\",\n        \"REMOVE\"\n      ]\n    },\n    \"isLastOp\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-propertygraph-stream-record-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: PropertygraphStreamRecord
---
