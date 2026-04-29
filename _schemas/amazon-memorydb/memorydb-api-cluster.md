---
description: An Amazon MemoryDB cluster.
layout: schema
name: Cluster
properties_list:
- description: The Amazon Resource Name (ARN) of the cluster.
  name: ARN
  type: string
- description: Indicates if the cluster has a Multi-AZ configuration.
  name: AvailabilityMode
  type: string
- description: A description of the cluster.
  name: Description
  type: string
- description: The Redis engine version the cluster is running.
  name: EngineVersion
  type: string
- description: The user-supplied name of the cluster.
  name: Name
  type: string
- description: The cluster's node type.
  name: NodeType
  type: string
- description: The number of shards in the cluster.
  name: NumberOfShards
  type: integer
- description: The status of the cluster.
  name: Status
  type: string
- description: A flag to indicate if In-transit encryption is enabled.
  name: TLSEnabled
  type: boolean
provider_name: Amazon MemoryDB
provider_slug: amazon-memorydb
schema_file: json-schema/memorydb-api-cluster-schema.json
slug: memorydb-api-cluster
source_filename: memorydb-api-cluster-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/json-schema/memorydb-api-cluster-schema.json\",\n  \"title\": \"Cluster\",\n  \"description\": \"An Amazon MemoryDB cluster.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ARN\": {\n      \"description\": \"The Amazon Resource Name (ARN) of the cluster.\",\n      \"type\": \"string\"\n    },\n    \"AvailabilityMode\": {\n      \"description\": \"Indicates if the cluster has a Multi-AZ configuration.\",\n      \"enum\": [\n        \"SingleAZ\",\n        \"MultiAZ\"\n      ],\n      \"type\": \"string\"\n    },\n    \"Description\": {\n      \"description\": \"A description of the cluster.\",\n      \"type\": \"string\"\n    },\n    \"EngineVersion\": {\n      \"description\": \"The Redis engine version the cluster is running.\",\n      \"type\": \"string\"\n    },\n    \"Name\": {\n      \"description\": \"\
  The user-supplied name of the cluster.\",\n      \"type\": \"string\"\n    },\n    \"NodeType\": {\n      \"description\": \"The cluster's node type.\",\n      \"type\": \"string\"\n    },\n    \"NumberOfShards\": {\n      \"description\": \"The number of shards in the cluster.\",\n      \"type\": \"integer\"\n    },\n    \"Status\": {\n      \"description\": \"The status of the cluster.\",\n      \"type\": \"string\"\n    },\n    \"TLSEnabled\": {\n      \"description\": \"A flag to indicate if In-transit encryption is enabled.\",\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/json-schema/memorydb-api-cluster-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Cluster
---
