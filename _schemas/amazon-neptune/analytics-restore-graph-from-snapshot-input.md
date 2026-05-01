---
description: RestoreGraphFromSnapshotInput schema from Neptune
layout: schema
name: RestoreGraphFromSnapshotInput
properties_list:
- description: The name of the restored graph.
  name: graphName
  type: string
- description: ''
  name: provisionedMemory
  type: integer
- description: ''
  name: deletionProtection
  type: boolean
- description: ''
  name: tags
  type: object
- description: ''
  name: replicaCount
  type: integer
- description: ''
  name: publicConnectivity
  type: boolean
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/analytics-restore-graph-from-snapshot-input-schema.json
slug: analytics-restore-graph-from-snapshot-input
source_filename: analytics-restore-graph-from-snapshot-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/analytics-restore-graph-from-snapshot-input-schema.json\",\n  \"title\": \"RestoreGraphFromSnapshotInput\",\n  \"description\": \"RestoreGraphFromSnapshotInput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"graphName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the restored graph.\"\n    },\n    \"provisionedMemory\": {\n      \"type\": \"integer\"\n    },\n    \"deletionProtection\": {\n      \"type\": \"boolean\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"replicaCount\": {\n      \"type\": \"integer\"\n    },\n    \"publicConnectivity\": {\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"graphName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/analytics-restore-graph-from-snapshot-input-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: RestoreGraphFromSnapshotInput
---
