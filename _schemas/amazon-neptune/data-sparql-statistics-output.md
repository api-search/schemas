---
description: SparqlStatisticsOutput schema from Neptune
layout: schema
name: SparqlStatisticsOutput
properties_list:
- description: ''
  name: status
  type: string
- description: ''
  name: payload
  type: object
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/data-sparql-statistics-output-schema.json
slug: data-sparql-statistics-output
source_filename: data-sparql-statistics-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-sparql-statistics-output-schema.json\",\n  \"title\": \"SparqlStatisticsOutput\",\n  \"description\": \"SparqlStatisticsOutput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"payload\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"graphStatistics\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"numStatements\": {\n              \"type\": \"integer\"\n            },\n            \"numDistinctSubjects\": {\n              \"type\": \"integer\"\n            },\n            \"numDistinctPredicates\": {\n              \"type\": \"integer\"\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-sparql-statistics-output-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: SparqlStatisticsOutput
---
