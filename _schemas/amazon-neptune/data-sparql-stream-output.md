---
description: SparqlStreamOutput schema from Neptune
layout: schema
name: SparqlStreamOutput
properties_list:
- description: ''
  name: lastEventId
  type: object
- description: ''
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
schema_file: json-schema/data-sparql-stream-output-schema.json
slug: data-sparql-stream-output
source_filename: data-sparql-stream-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-sparql-stream-output-schema.json\",\n  \"title\": \"SparqlStreamOutput\",\n  \"description\": \"SparqlStreamOutput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lastEventId\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"commitNum\": {\n          \"type\": \"integer\"\n        },\n        \"opNum\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"lastTrxTimestampInMillis\": {\n      \"type\": \"integer\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"NQUADS\"\n      ]\n    },\n    \"records\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"commitTimestampInMillis\": {\n            \"type\": \"integer\"\n          },\n\
  \          \"eventId\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"commitNum\": {\n                \"type\": \"integer\"\n              },\n              \"opNum\": {\n                \"type\": \"integer\"\n              }\n            }\n          },\n          \"data\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"stmt\": {\n                \"type\": \"string\",\n                \"description\": \"The N-Quads statement.\"\n              }\n            }\n          },\n          \"op\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"ADD\",\n              \"REMOVE\"\n            ]\n          },\n          \"isLastOp\": {\n            \"type\": \"boolean\"\n          }\n        }\n      }\n    },\n    \"totalRecords\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-sparql-stream-output-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: SparqlStreamOutput
---
