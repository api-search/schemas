---
description: OpenCypherQueryStatusOutput schema from Neptune
layout: schema
name: OpenCypherQueryStatusOutput
properties_list:
- description: ''
  name: acceptedQueryCount
  type: integer
- description: ''
  name: runningQueryCount
  type: integer
- description: ''
  name: queries
  type: array
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/data-open-cypher-query-status-output-schema.json
slug: data-open-cypher-query-status-output
source_filename: data-open-cypher-query-status-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-open-cypher-query-status-output-schema.json\",\n  \"title\": \"OpenCypherQueryStatusOutput\",\n  \"description\": \"OpenCypherQueryStatusOutput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"acceptedQueryCount\": {\n      \"type\": \"integer\"\n    },\n    \"runningQueryCount\": {\n      \"type\": \"integer\"\n    },\n    \"queries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"queryId\": {\n            \"type\": \"string\"\n          },\n          \"queryString\": {\n            \"type\": \"string\"\n          },\n          \"queryEvalStats\": {\n            \"type\": \"object\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-open-cypher-query-status-output-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: OpenCypherQueryStatusOutput
---
