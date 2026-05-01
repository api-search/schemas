---
description: SPARQL 1.1 Query Results JSON Format as defined by W3C.
layout: schema
name: SparqlSelectResponse
properties_list:
- description: ''
  name: head
  type: object
- description: ''
  name: results
  type: object
- description: The result for ASK queries.
  name: boolean
  type: boolean
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/sparql-sparql-select-response-schema.json
slug: sparql-sparql-select-response
source_filename: sparql-sparql-select-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/sparql-sparql-select-response-schema.json\",\n  \"title\": \"SparqlSelectResponse\",\n  \"description\": \"SPARQL 1.1 Query Results JSON Format as defined by W3C.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"head\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"vars\": {\n          \"type\": \"array\",\n          \"description\": \"The list of variable names in the result set.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"link\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"results\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"bindings\": {\n          \"type\": \"array\",\n          \"description\": \"The\
  \ result bindings for each solution.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"additionalProperties\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"type\": {\n                  \"type\": \"string\",\n                  \"enum\": [\n                    \"uri\",\n                    \"literal\",\n                    \"bnode\"\n                  ]\n                },\n                \"value\": {\n                  \"type\": \"string\"\n                },\n                \"datatype\": {\n                  \"type\": \"string\"\n                },\n                \"xml:lang\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"boolean\": {\n      \"type\": \"boolean\",\n      \"description\": \"The result for ASK queries.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/sparql-sparql-select-response-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: SparqlSelectResponse
---
