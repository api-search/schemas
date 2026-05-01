---
description: CreateGraphInput schema from Neptune
layout: schema
name: CreateGraphInput
properties_list:
- description: The name of the graph (1-63 alphanumeric characters or hyphens).
  name: graphName
  type: string
- description: The provisioned memory size in Neptune Capacity Units (NCUs).
  name: provisionedMemory
  type: integer
- description: Tags to assign to the graph.
  name: tags
  type: object
- description: Whether the graph can be reached over the internet.
  name: publicConnectivity
  type: boolean
- description: KMS key identifier for encryption at rest.
  name: kmsKeyIdentifier
  type: string
- description: Vector search configuration for the graph.
  name: vectorSearchConfiguration
  type: object
- description: The number of read replicas.
  name: replicaCount
  type: integer
- description: Whether deletion protection is enabled.
  name: deletionProtection
  type: boolean
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/analytics-create-graph-input-schema.json
slug: analytics-create-graph-input
source_filename: analytics-create-graph-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/analytics-create-graph-input-schema.json\",\n  \"title\": \"CreateGraphInput\",\n  \"description\": \"CreateGraphInput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"graphName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the graph (1-63 alphanumeric characters or hyphens).\",\n      \"minLength\": 1,\n      \"maxLength\": 63\n    },\n    \"provisionedMemory\": {\n      \"type\": \"integer\",\n      \"description\": \"The provisioned memory size in Neptune Capacity Units (NCUs).\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags to assign to the graph.\"\n    },\n    \"publicConnectivity\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether the graph can be reached over the internet.\",\n      \"default\": false\n    },\n    \"kmsKeyIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"KMS key identifier for encryption at rest.\"\n    },\n    \"vectorSearchConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"Vector search configuration for the graph.\",\n      \"properties\": {\n        \"dimension\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of dimensions for vector embeddings.\"\n        }\n      }\n    },\n    \"replicaCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of read replicas.\",\n      \"default\": 0\n    },\n    \"deletionProtection\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether deletion protection is enabled.\",\n      \"default\": false\n    }\n  },\n  \"required\": [\n    \"graphName\",\n    \"provisionedMemory\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/analytics-create-graph-input-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: CreateGraphInput
---
