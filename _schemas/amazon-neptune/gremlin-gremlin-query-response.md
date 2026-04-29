---
description: GremlinQueryResponse schema from Neptune
layout: schema
name: GremlinQueryResponse
properties_list:
- description: The unique request identifier.
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
schema_file: json-schema/gremlin-gremlin-query-response-schema.json
slug: gremlin-gremlin-query-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/gremlin-gremlin-query-response-schema.json\",\n  \"title\": \"GremlinQueryResponse\",\n  \"description\": \"GremlinQueryResponse schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique request identifier.\"\n    },\n    \"status\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"message\": {\n          \"type\": \"string\"\n        },\n        \"code\": {\n          \"type\": \"integer\",\n          \"description\": \"The response status code (200 for success).\"\n        },\n        \"attributes\": {\n          \"type\": \"object\",\n          \"description\": \"Additional response attributes.\"\n        }\n      }\n    },\n    \"result\": {\n      \"type\"\
  : \"object\",\n      \"properties\": {\n        \"data\": {\n          \"description\": \"The query result data. The shape depends on the traversal's terminal step (e.g., count, valueMap, path).\"\n        },\n        \"meta\": {\n          \"type\": \"object\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/gremlin-gremlin-query-response-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: GremlinQueryResponse
---
