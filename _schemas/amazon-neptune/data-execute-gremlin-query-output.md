---
description: ExecuteGremlinQueryOutput schema from Neptune
layout: schema
name: ExecuteGremlinQueryOutput
properties_list:
- description: ''
  name: requestId
  type: string
- description: ''
  name: status
  type: object
- description: ''
  name: result
  type: object
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/data-execute-gremlin-query-output-schema.json
slug: data-execute-gremlin-query-output
source_filename: data-execute-gremlin-query-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-execute-gremlin-query-output-schema.json\",\n  \"title\": \"ExecuteGremlinQueryOutput\",\n  \"description\": \"ExecuteGremlinQueryOutput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"message\": {\n          \"type\": \"string\"\n        },\n        \"code\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"result\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"data\": {\n          \"description\": \"The query result data.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-execute-gremlin-query-output-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: ExecuteGremlinQueryOutput
---
