---
description: ListGraphSnapshotsOutput schema from Neptune
layout: schema
name: ListGraphSnapshotsOutput
properties_list:
- description: ''
  name: graphSnapshots
  type: array
- description: ''
  name: nextToken
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/analytics-list-graph-snapshots-output-schema.json
slug: analytics-list-graph-snapshots-output
source_filename: analytics-list-graph-snapshots-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/analytics-list-graph-snapshots-output-schema.json\",\n  \"title\": \"ListGraphSnapshotsOutput\",\n  \"description\": \"ListGraphSnapshotsOutput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"graphSnapshots\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"arn\": {\n            \"type\": \"string\"\n          },\n          \"sourceGraphId\": {\n            \"type\": \"string\"\n          },\n          \"snapshotCreateTime\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"status\": {\n            \"type\": \"string\"\
  \n          }\n        }\n      }\n    },\n    \"nextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/analytics-list-graph-snapshots-output-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: ListGraphSnapshotsOutput
---
