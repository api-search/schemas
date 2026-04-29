---
description: ExecuteGremlinQueryInput schema from Neptune
layout: schema
name: ExecuteGremlinQueryInput
properties_list:
- description: The Gremlin traversal query string to execute.
  name: gremlin
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/data-execute-gremlin-query-input-schema.json
slug: data-execute-gremlin-query-input
source_filename: data-execute-gremlin-query-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-execute-gremlin-query-input-schema.json\",\n  \"title\": \"ExecuteGremlinQueryInput\",\n  \"description\": \"ExecuteGremlinQueryInput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"gremlin\": {\n      \"type\": \"string\",\n      \"description\": \"The Gremlin traversal query string to execute.\"\n    }\n  },\n  \"required\": [\n    \"gremlin\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-execute-gremlin-query-input-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: ExecuteGremlinQueryInput
---
