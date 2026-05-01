---
description: GremlinQueryStatus schema from Neptune
layout: schema
name: GremlinQueryStatus
properties_list:
- description: ''
  name: queryId
  type: string
- description: ''
  name: queryString
  type: string
- description: ''
  name: queryEvalStats
  type: object
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/data-gremlin-query-status-schema.json
slug: data-gremlin-query-status
source_filename: data-gremlin-query-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-gremlin-query-status-schema.json\",\n  \"title\": \"GremlinQueryStatus\",\n  \"description\": \"GremlinQueryStatus schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"queryId\": {\n      \"type\": \"string\"\n    },\n    \"queryString\": {\n      \"type\": \"string\"\n    },\n    \"queryEvalStats\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"waited\": {\n          \"type\": \"integer\"\n        },\n        \"elapsed\": {\n          \"type\": \"integer\"\n        },\n        \"cancelled\": {\n          \"type\": \"boolean\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-gremlin-query-status-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: GremlinQueryStatus
---
