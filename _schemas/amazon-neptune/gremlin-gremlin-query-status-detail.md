---
description: GremlinQueryStatusDetail schema from Neptune
layout: schema
name: GremlinQueryStatusDetail
properties_list:
- description: The unique query identifier.
  name: queryId
  type: string
- description: The Gremlin traversal query string.
  name: queryString
  type: string
- description: Query execution statistics.
  name: queryEvalStats
  type: object
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/gremlin-gremlin-query-status-detail-schema.json
slug: gremlin-gremlin-query-status-detail
source_filename: gremlin-gremlin-query-status-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/gremlin-gremlin-query-status-detail-schema.json\",\n  \"title\": \"GremlinQueryStatusDetail\",\n  \"description\": \"GremlinQueryStatusDetail schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"queryId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique query identifier.\"\n    },\n    \"queryString\": {\n      \"type\": \"string\",\n      \"description\": \"The Gremlin traversal query string.\"\n    },\n    \"queryEvalStats\": {\n      \"type\": \"object\",\n      \"description\": \"Query execution statistics.\",\n      \"properties\": {\n        \"waited\": {\n          \"type\": \"integer\",\n          \"description\": \"The time the query waited in the queue (milliseconds).\"\n        },\n        \"elapsed\": {\n          \"type\": \"integer\",\n          \"\
  description\": \"The elapsed execution time (milliseconds).\"\n        },\n        \"cancelled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the query was cancelled.\"\n        },\n        \"subqueries\": {\n          \"type\": \"object\",\n          \"description\": \"Statistics for subqueries, if any.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/gremlin-gremlin-query-status-detail-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: GremlinQueryStatusDetail
---
