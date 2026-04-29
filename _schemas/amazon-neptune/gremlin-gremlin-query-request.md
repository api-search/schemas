---
description: GremlinQueryRequest schema from Neptune
layout: schema
name: GremlinQueryRequest
properties_list:
- description: The Gremlin traversal query string. Must be a valid Gremlin traversal starting with g. The bindings property is not supported by Neptune.
  name: gremlin
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/gremlin-gremlin-query-request-schema.json
slug: gremlin-gremlin-query-request
source_filename: gremlin-gremlin-query-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/gremlin-gremlin-query-request-schema.json\",\n  \"title\": \"GremlinQueryRequest\",\n  \"description\": \"GremlinQueryRequest schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"gremlin\": {\n      \"type\": \"string\",\n      \"description\": \"The Gremlin traversal query string. Must be a valid Gremlin traversal starting with g. The bindings property is not supported by Neptune.\",\n      \"examples\": [\n        \"g.V().count()\",\n        \"g.V().has('name','John').out('knows')\"\n      ]\n    }\n  },\n  \"required\": [\n    \"gremlin\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/gremlin-gremlin-query-request-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: GremlinQueryRequest
---
