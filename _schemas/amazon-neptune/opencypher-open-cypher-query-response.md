---
description: OpenCypherQueryResponse schema from Neptune
layout: schema
name: OpenCypherQueryResponse
properties_list:
- description: The query result rows.
  name: results
  type: array
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/opencypher-open-cypher-query-response-schema.json
slug: opencypher-open-cypher-query-response
source_filename: opencypher-open-cypher-query-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/opencypher-open-cypher-query-response-schema.json\",\n  \"title\": \"OpenCypherQueryResponse\",\n  \"description\": \"OpenCypherQueryResponse schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"The query result rows.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A result row. Keys are the RETURN alias names. Values can be scalars, nodes, relationships, or paths.\",\n        \"additionalProperties\": {\n          \"description\": \"Result value. Nodes have ~id, ~entityType, ~labels, ~properties. Relationships have ~id, ~entityType, ~start, ~end, ~type, ~properties.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/opencypher-open-cypher-query-response-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: OpenCypherQueryResponse
---
