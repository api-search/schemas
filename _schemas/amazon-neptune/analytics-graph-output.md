---
description: GraphOutput schema from Neptune
layout: schema
name: GraphOutput
properties_list:
- description: The unique identifier of the graph.
  name: id
  type: string
- description: The name of the graph.
  name: name
  type: string
- description: The ARN of the graph.
  name: arn
  type: string
- description: The current status of the graph.
  name: status
  type: string
- description: ''
  name: statusReason
  type: string
- description: ''
  name: createTime
  type: string
- description: ''
  name: provisionedMemory
  type: integer
- description: The DNS endpoint for the graph.
  name: endpoint
  type: string
- description: ''
  name: publicConnectivity
  type: boolean
- description: ''
  name: vectorSearchConfiguration
  type: object
- description: ''
  name: replicaCount
  type: integer
- description: ''
  name: kmsKeyIdentifier
  type: string
- description: ''
  name: sourceSnapshotId
  type: string
- description: ''
  name: deletionProtection
  type: boolean
- description: ''
  name: buildNumber
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/analytics-graph-output-schema.json
slug: analytics-graph-output
source_filename: analytics-graph-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/analytics-graph-output-schema.json\",\n  \"title\": \"GraphOutput\",\n  \"description\": \"GraphOutput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the graph.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the graph.\"\n    },\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the graph.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the graph.\",\n      \"enum\": [\n        \"CREATING\",\n        \"AVAILABLE\",\n        \"DELETING\",\n        \"RESETTING\",\n        \"UPDATING\",\n        \"SNAPSHOTTING\",\n        \"FAILED\",\n        \"IMPORTING\"\n\
  \      ]\n    },\n    \"statusReason\": {\n      \"type\": \"string\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"provisionedMemory\": {\n      \"type\": \"integer\"\n    },\n    \"endpoint\": {\n      \"type\": \"string\",\n      \"description\": \"The DNS endpoint for the graph.\"\n    },\n    \"publicConnectivity\": {\n      \"type\": \"boolean\"\n    },\n    \"vectorSearchConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"dimension\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"replicaCount\": {\n      \"type\": \"integer\"\n    },\n    \"kmsKeyIdentifier\": {\n      \"type\": \"string\"\n    },\n    \"sourceSnapshotId\": {\n      \"type\": \"string\"\n    },\n    \"deletionProtection\": {\n      \"type\": \"boolean\"\n    },\n    \"buildNumber\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/analytics-graph-output-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: GraphOutput
---
