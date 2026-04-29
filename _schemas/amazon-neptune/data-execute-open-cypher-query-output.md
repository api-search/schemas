---
description: ExecuteOpenCypherQueryOutput schema from Neptune
layout: schema
name: ExecuteOpenCypherQueryOutput
properties_list:
- description: The query result rows.
  name: results
  type: array
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/data-execute-open-cypher-query-output-schema.json
slug: data-execute-open-cypher-query-output
source_filename: data-execute-open-cypher-query-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-execute-open-cypher-query-output-schema.json\",\n  \"title\": \"ExecuteOpenCypherQueryOutput\",\n  \"description\": \"ExecuteOpenCypherQueryOutput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"The query result rows.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-execute-open-cypher-query-output-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: ExecuteOpenCypherQueryOutput
---
