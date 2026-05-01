---
description: ExecuteSparqlQueryInput schema from Neptune
layout: schema
name: ExecuteSparqlQueryInput
properties_list:
- description: The SPARQL query string (for SELECT, ASK, CONSTRUCT, DESCRIBE).
  name: query
  type: string
- description: The SPARQL update string (for INSERT, DELETE operations).
  name: update
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/data-execute-sparql-query-input-schema.json
slug: data-execute-sparql-query-input
source_filename: data-execute-sparql-query-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-execute-sparql-query-input-schema.json\",\n  \"title\": \"ExecuteSparqlQueryInput\",\n  \"description\": \"ExecuteSparqlQueryInput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"The SPARQL query string (for SELECT, ASK, CONSTRUCT, DESCRIBE).\"\n    },\n    \"update\": {\n      \"type\": \"string\",\n      \"description\": \"The SPARQL update string (for INSERT, DELETE operations).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-execute-sparql-query-input-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: ExecuteSparqlQueryInput
---
