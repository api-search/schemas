---
description: SparqlQueryOutput schema from Neptune
layout: schema
name: SparqlQueryOutput
properties_list:
- description: ''
  name: head
  type: object
- description: ''
  name: results
  type: object
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/data-sparql-query-output-schema.json
slug: data-sparql-query-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-sparql-query-output-schema.json\",\n  \"title\": \"SparqlQueryOutput\",\n  \"description\": \"SparqlQueryOutput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"head\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"vars\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"results\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"bindings\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-sparql-query-output-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: SparqlQueryOutput
---
