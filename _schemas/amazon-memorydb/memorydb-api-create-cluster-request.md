---
description: CreateClusterRequest schema from Amazon MemoryDB API
layout: schema
name: CreateClusterRequest
properties_list:
- description: The name of the Access Control List to associate with the cluster.
  name: ACLName
  type: string
- description: The name of the cluster.
  name: ClusterName
  type: string
- description: An optional description of the cluster.
  name: Description
  type: string
- description: The version number of the Redis engine to use.
  name: EngineVersion
  type: string
- description: The compute and memory capacity of the nodes.
  name: NodeType
  type: string
- description: The number of replicas to apply to each shard.
  name: NumReplicasPerShard
  type: integer
- description: The number of shards the cluster will contain.
  name: NumShards
  type: integer
- description: A flag to enable in-transit encryption.
  name: TLSEnabled
  type: boolean
provider_name: Amazon MemoryDB
provider_slug: amazon-memorydb
schema_file: json-schema/memorydb-api-create-cluster-request-schema.json
slug: memorydb-api-create-cluster-request
source_filename: memorydb-api-create-cluster-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/json-schema/memorydb-api-create-cluster-request-schema.json\",\n  \"title\": \"CreateClusterRequest\",\n  \"description\": \"CreateClusterRequest schema from Amazon MemoryDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ACLName\": {\n      \"description\": \"The name of the Access Control List to associate with the cluster.\",\n      \"type\": \"string\"\n    },\n    \"ClusterName\": {\n      \"description\": \"The name of the cluster.\",\n      \"type\": \"string\"\n    },\n    \"Description\": {\n      \"description\": \"An optional description of the cluster.\",\n      \"type\": \"string\"\n    },\n    \"EngineVersion\": {\n      \"description\": \"The version number of the Redis engine to use.\",\n      \"type\": \"string\"\n    },\n    \"NodeType\": {\n      \"description\": \"The compute and memory\
  \ capacity of the nodes.\",\n      \"type\": \"string\"\n    },\n    \"NumReplicasPerShard\": {\n      \"description\": \"The number of replicas to apply to each shard.\",\n      \"type\": \"integer\"\n    },\n    \"NumShards\": {\n      \"description\": \"The number of shards the cluster will contain.\",\n      \"type\": \"integer\"\n    },\n    \"TLSEnabled\": {\n      \"description\": \"A flag to enable in-transit encryption.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"ClusterName\",\n    \"NodeType\",\n    \"ACLName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/json-schema/memorydb-api-create-cluster-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CreateClusterRequest
---
