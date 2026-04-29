---
description: CreateGraphSnapshotInput schema from Neptune
layout: schema
name: CreateGraphSnapshotInput
properties_list:
- description: The identifier of the graph to snapshot.
  name: graphIdentifier
  type: string
- description: The name of the snapshot.
  name: snapshotName
  type: string
- description: ''
  name: tags
  type: object
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/analytics-create-graph-snapshot-input-schema.json
slug: analytics-create-graph-snapshot-input
source_filename: analytics-create-graph-snapshot-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/analytics-create-graph-snapshot-input-schema.json\",\n  \"title\": \"CreateGraphSnapshotInput\",\n  \"description\": \"CreateGraphSnapshotInput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"graphIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the graph to snapshot.\"\n    },\n    \"snapshotName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the snapshot.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"graphIdentifier\",\n    \"snapshotName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/analytics-create-graph-snapshot-input-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: CreateGraphSnapshotInput
---
