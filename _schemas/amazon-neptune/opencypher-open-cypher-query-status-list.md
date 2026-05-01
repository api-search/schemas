---
description: OpenCypherQueryStatusList schema from Neptune
layout: schema
name: OpenCypherQueryStatusList
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
schema_file: json-schema/opencypher-open-cypher-query-status-list-schema.json
slug: opencypher-open-cypher-query-status-list
source_filename: opencypher-open-cypher-query-status-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/opencypher-open-cypher-query-status-list-schema.json\",\n  \"title\": \"OpenCypherQueryStatusList\",\n  \"description\": \"OpenCypherQueryStatusList schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"acceptedQueryCount\": {\n      \"type\": \"integer\"\n    },\n    \"runningQueryCount\": {\n      \"type\": \"integer\"\n    },\n    \"queries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/OpenCypherQueryStatusDetail\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/opencypher-open-cypher-query-status-list-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: OpenCypherQueryStatusList
---
