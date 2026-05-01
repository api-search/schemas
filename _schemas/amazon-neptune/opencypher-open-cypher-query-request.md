---
description: OpenCypherQueryRequest schema from Neptune
layout: schema
name: OpenCypherQueryRequest
properties_list:
- description: The openCypher query string.
  name: query
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/opencypher-open-cypher-query-request-schema.json
slug: opencypher-open-cypher-query-request
source_filename: opencypher-open-cypher-query-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/opencypher-open-cypher-query-request-schema.json\",\n  \"title\": \"OpenCypherQueryRequest\",\n  \"description\": \"OpenCypherQueryRequest schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"The openCypher query string.\"\n    }\n  },\n  \"required\": [\n    \"query\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/opencypher-open-cypher-query-request-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: OpenCypherQueryRequest
---
