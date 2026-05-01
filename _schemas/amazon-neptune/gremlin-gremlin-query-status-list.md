---
description: GremlinQueryStatusList schema from Neptune
layout: schema
name: GremlinQueryStatusList
properties_list:
- description: The total number of accepted queries.
  name: acceptedQueryCount
  type: integer
- description: The number of currently running queries.
  name: runningQueryCount
  type: integer
- description: The list of running and waiting queries.
  name: queries
  type: array
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/gremlin-gremlin-query-status-list-schema.json
slug: gremlin-gremlin-query-status-list
source_filename: gremlin-gremlin-query-status-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/gremlin-gremlin-query-status-list-schema.json\",\n  \"title\": \"GremlinQueryStatusList\",\n  \"description\": \"GremlinQueryStatusList schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"acceptedQueryCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of accepted queries.\"\n    },\n    \"runningQueryCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of currently running queries.\"\n    },\n    \"queries\": {\n      \"type\": \"array\",\n      \"description\": \"The list of running and waiting queries.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/GremlinQueryStatusDetail\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/gremlin-gremlin-query-status-list-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: GremlinQueryStatusList
---
