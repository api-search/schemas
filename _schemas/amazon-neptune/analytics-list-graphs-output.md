---
description: ListGraphsOutput schema from Neptune
layout: schema
name: ListGraphsOutput
properties_list:
- description: ''
  name: graphs
  type: array
- description: ''
  name: nextToken
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/analytics-list-graphs-output-schema.json
slug: analytics-list-graphs-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/analytics-list-graphs-output-schema.json\",\n  \"title\": \"ListGraphsOutput\",\n  \"description\": \"ListGraphsOutput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"graphs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"arn\": {\n            \"type\": \"string\"\n          },\n          \"status\": {\n            \"type\": \"string\"\n          },\n          \"provisionedMemory\": {\n            \"type\": \"integer\"\n          },\n          \"publicConnectivity\": {\n            \"type\": \"boolean\"\n          },\n          \"endpoint\": {\n            \"type\"\
  : \"string\"\n          },\n          \"replicaCount\": {\n            \"type\": \"integer\"\n          },\n          \"deletionProtection\": {\n            \"type\": \"boolean\"\n          }\n        }\n      }\n    },\n    \"nextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/analytics-list-graphs-output-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: ListGraphsOutput
---
