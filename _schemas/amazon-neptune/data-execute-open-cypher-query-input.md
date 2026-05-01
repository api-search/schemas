---
description: ExecuteOpenCypherQueryInput schema from Neptune
layout: schema
name: ExecuteOpenCypherQueryInput
properties_list:
- description: The openCypher query string to execute.
  name: query
  type: string
- description: The openCypher query parameters as a JSON-serialized string.
  name: parameters
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/data-execute-open-cypher-query-input-schema.json
slug: data-execute-open-cypher-query-input
source_filename: data-execute-open-cypher-query-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-execute-open-cypher-query-input-schema.json\",\n  \"title\": \"ExecuteOpenCypherQueryInput\",\n  \"description\": \"ExecuteOpenCypherQueryInput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"The openCypher query string to execute.\"\n    },\n    \"parameters\": {\n      \"type\": \"string\",\n      \"description\": \"The openCypher query parameters as a JSON-serialized string.\"\n    }\n  },\n  \"required\": [\n    \"query\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-execute-open-cypher-query-input-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: ExecuteOpenCypherQueryInput
---
