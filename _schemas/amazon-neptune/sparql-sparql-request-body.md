---
description: SparqlRequestBody schema from Neptune
layout: schema
name: SparqlRequestBody
properties_list:
- description: A SPARQL 1.1 query (SELECT, ASK, CONSTRUCT, or DESCRIBE). Mutually exclusive with update.
  name: query
  type: string
- description: A SPARQL 1.1 Update operation (INSERT DATA, DELETE DATA, etc.). Mutually exclusive with query.
  name: update
  type: string
- description: Default graph URI for the query.
  name: using-graph-uri
  type: string
- description: Named graph URI for the query.
  name: using-named-graph-uri
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/sparql-sparql-request-body-schema.json
slug: sparql-sparql-request-body
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/sparql-sparql-request-body-schema.json\",\n  \"title\": \"SparqlRequestBody\",\n  \"description\": \"SparqlRequestBody schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"A SPARQL 1.1 query (SELECT, ASK, CONSTRUCT, or DESCRIBE). Mutually exclusive with update.\"\n    },\n    \"update\": {\n      \"type\": \"string\",\n      \"description\": \"A SPARQL 1.1 Update operation (INSERT DATA, DELETE DATA, etc.). Mutually exclusive with query.\"\n    },\n    \"using-graph-uri\": {\n      \"type\": \"string\",\n      \"description\": \"Default graph URI for the query.\"\n    },\n    \"using-named-graph-uri\": {\n      \"type\": \"string\",\n      \"description\": \"Named graph URI for the query.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/sparql-sparql-request-body-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: SparqlRequestBody
---
