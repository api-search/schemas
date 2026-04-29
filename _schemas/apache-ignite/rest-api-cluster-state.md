---
description: Information about current cluster state.
layout: schema
name: ClusterState
properties_list:
- description: List of cluster management group nodes. These nodes are responsible for maintaining RAFT cluster topology.
  name: cmgNodes
  type: array
- description: List of metastorage nodes. These nodes are responsible for storing RAFT cluster metadata.
  name: msNodes
  type: array
- description: Version of Apache Ignite that the cluster was created on.
  name: igniteVersion
  type: string
- description: ''
  name: clusterTag
  type: object
- description: IDs the cluster had before.
  name: formerClusterIds
  type: array
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-cluster-state-schema.json
slug: rest-api-cluster-state
source_filename: rest-api-cluster-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-cluster-state-schema.json\",\n  \"title\": \"ClusterState\",\n  \"description\": \"Information about current cluster state.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cmgNodes\": {\n      \"type\": \"array\",\n      \"description\": \"List of cluster management group nodes. These nodes are responsible for maintaining RAFT cluster topology.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"msNodes\": {\n      \"type\": \"array\",\n      \"description\": \"List of metastorage nodes. These nodes are responsible for storing RAFT cluster metadata.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"igniteVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Version of Apache Ignite that the cluster was created on.\"\n    },\n\
  \    \"clusterTag\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClusterTag\"\n        },\n        {\n          \"description\": \"Unique tag that identifies the cluster.\"\n        }\n      ]\n    },\n    \"formerClusterIds\": {\n      \"type\": \"array\",\n      \"description\": \"IDs the cluster had before.\",\n      \"nullable\": true,\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uuid\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-cluster-state-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: ClusterState
---
