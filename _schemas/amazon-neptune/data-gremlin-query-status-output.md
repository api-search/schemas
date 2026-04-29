---
description: GremlinQueryStatusOutput schema from Neptune
layout: schema
name: GremlinQueryStatusOutput
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
schema_file: json-schema/data-gremlin-query-status-output-schema.json
slug: data-gremlin-query-status-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-gremlin-query-status-output-schema.json\",\n  \"title\": \"GremlinQueryStatusOutput\",\n  \"description\": \"GremlinQueryStatusOutput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"acceptedQueryCount\": {\n      \"type\": \"integer\"\n    },\n    \"runningQueryCount\": {\n      \"type\": \"integer\"\n    },\n    \"queries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/GremlinQueryStatus\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-gremlin-query-status-output-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: GremlinQueryStatusOutput
---
