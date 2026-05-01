---
description: Represents a Neptune Analytics graph resource, which is a memory-optimized graph database instance for analytical workloads with support for openCypher queries, vector search, and optimized graph algorithms.
layout: schema
name: Amazon Neptune Analytics Graph
properties_list:
- description: The unique identifier of the graph, assigned by Neptune Analytics.
  name: id
  type: string
- description: The name of the graph.
  name: name
  type: string
- description: The name of the graph (used in creation requests).
  name: graphName
  type: string
- description: The Amazon Resource Name (ARN) of the graph.
  name: arn
  type: string
- description: The current status of the graph resource.
  name: status
  type: string
- description: The reason for the current status, if applicable.
  name: statusReason
  type: string
- description: The time the graph was created.
  name: createTime
  type: string
- description: The provisioned memory size in Neptune Capacity Units (NCUs). Each NCU provides approximately 2 GiB of memory.
  name: provisionedMemory
  type: integer
- description: The DNS endpoint for connecting to the graph.
  name: endpoint
  type: string
- description: Whether the graph can be accessed over the public internet.
  name: publicConnectivity
  type: boolean
- description: Configuration for vector search capabilities.
  name: vectorSearchConfiguration
  type: object
- description: The number of read replicas for the graph.
  name: replicaCount
  type: integer
- description: The KMS key identifier used for encryption at rest.
  name: kmsKeyIdentifier
  type: string
- description: The ID of the source snapshot if the graph was restored from a snapshot.
  name: sourceSnapshotId
  type: string
- description: Whether deletion protection is enabled for the graph.
  name: deletionProtection
  type: boolean
- description: The build number of the Neptune Analytics engine.
  name: buildNumber
  type: string
- description: Tags assigned to the graph as key-value pairs.
  name: tags
  type: object
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/amazon-neptune-analytics-graph-schema.json
slug: amazon-neptune-analytics-graph
source_filename: amazon-neptune-analytics-graph-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/amazon-neptune/json-schema/amazon-neptune-analytics-graph-schema.json\",\n  \"title\": \"Amazon Neptune Analytics Graph\",\n  \"description\": \"Represents a Neptune Analytics graph resource, which is a memory-optimized graph database instance for analytical workloads with support for openCypher queries, vector search, and optimized graph algorithms.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"graphName\",\n    \"provisionedMemory\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the graph, assigned by Neptune Analytics.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the graph.\",\n      \"minLength\": 1,\n      \"maxLength\": 63,\n      \"pattern\": \"^[a-zA-Z][a-zA-Z0-9-]*$\"\n    },\n    \"graphName\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The name of the graph (used in creation requests).\",\n      \"minLength\": 1,\n      \"maxLength\": 63\n    },\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the graph.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the graph resource.\",\n      \"enum\": [\n        \"CREATING\",\n        \"AVAILABLE\",\n        \"DELETING\",\n        \"RESETTING\",\n        \"UPDATING\",\n        \"SNAPSHOTTING\",\n        \"FAILED\",\n        \"IMPORTING\"\n      ]\n    },\n    \"statusReason\": {\n      \"type\": \"string\",\n      \"description\": \"The reason for the current status, if applicable.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the graph was created.\"\n    },\n    \"provisionedMemory\": {\n      \"type\": \"integer\",\n      \"description\": \"The provisioned\
  \ memory size in Neptune Capacity Units (NCUs). Each NCU provides approximately 2 GiB of memory.\",\n      \"minimum\": 16\n    },\n    \"endpoint\": {\n      \"type\": \"string\",\n      \"description\": \"The DNS endpoint for connecting to the graph.\"\n    },\n    \"publicConnectivity\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the graph can be accessed over the public internet.\",\n      \"default\": false\n    },\n    \"vectorSearchConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for vector search capabilities.\",\n      \"properties\": {\n        \"dimension\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of dimensions for vector embeddings.\",\n          \"minimum\": 1\n        }\n      }\n    },\n    \"replicaCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of read replicas for the graph.\",\n      \"minimum\": 0,\n      \"default\": 0\n    },\n    \"kmsKeyIdentifier\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The KMS key identifier used for encryption at rest.\"\n    },\n    \"sourceSnapshotId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the source snapshot if the graph was restored from a snapshot.\"\n    },\n    \"deletionProtection\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether deletion protection is enabled for the graph.\",\n      \"default\": false\n    },\n    \"buildNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The build number of the Neptune Analytics engine.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Tags assigned to the graph as key-value pairs.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/amazon-neptune-analytics-graph-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: Amazon Neptune Analytics Graph
---
