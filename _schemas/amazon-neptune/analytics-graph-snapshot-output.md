---
description: GraphSnapshotOutput schema from Neptune
layout: schema
name: GraphSnapshotOutput
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: arn
  type: string
- description: ''
  name: sourceGraphId
  type: string
- description: ''
  name: snapshotCreateTime
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: kmsKeyIdentifier
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/analytics-graph-snapshot-output-schema.json
slug: analytics-graph-snapshot-output
source_filename: analytics-graph-snapshot-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/analytics-graph-snapshot-output-schema.json\",\n  \"title\": \"GraphSnapshotOutput\",\n  \"description\": \"GraphSnapshotOutput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"arn\": {\n      \"type\": \"string\"\n    },\n    \"sourceGraphId\": {\n      \"type\": \"string\"\n    },\n    \"snapshotCreateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CREATING\",\n        \"AVAILABLE\",\n        \"DELETING\",\n        \"FAILED\"\n      ]\n    },\n    \"kmsKeyIdentifier\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/analytics-graph-snapshot-output-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: GraphSnapshotOutput
---
