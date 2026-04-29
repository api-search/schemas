---
description: SPARQL query results in JSON format
layout: schema
name: SparqlResults
properties_list:
- description: Result metadata including variable names
  name: head
  type: object
- description: Query result bindings
  name: results
  type: object
- description: Result for ASK queries
  name: boolean
  type: boolean
provider_name: Apache Jena
provider_slug: apache-jena
schema_file: json-schema/fuseki-sparql-api-sparql-results-schema.json
slug: fuseki-sparql-api-sparql-results
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-jena/refs/heads/main/json-schema/fuseki-sparql-api-sparql-results-schema.json\",\n  \"title\": \"SparqlResults\",\n  \"description\": \"SPARQL query results in JSON format\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"head\": {\n      \"type\": \"object\",\n      \"description\": \"Result metadata including variable names\",\n      \"properties\": {\n        \"vars\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"example\": [\n            \"s\",\n            \"p\",\n            \"o\"\n          ]\n        }\n      }\n    },\n    \"results\": {\n      \"type\": \"object\",\n      \"description\": \"Query result bindings\",\n      \"properties\": {\n        \"bindings\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/Binding\"\
  \n          }\n        }\n      }\n    },\n    \"boolean\": {\n      \"type\": \"boolean\",\n      \"description\": \"Result for ASK queries\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-jena/refs/heads/main/json-schema/fuseki-sparql-api-sparql-results-schema.json
tags:
- Java
- Linked Data
- OWL
- Ontology
- Open Source
- RDF
- Semantic Web
- SPARQL
title: SparqlResults
---
