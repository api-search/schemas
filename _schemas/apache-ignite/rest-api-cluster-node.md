---
description: Information about the cluster node.
layout: schema
name: ClusterNode
properties_list:
- description: Node ID.
  name: id
  type: string
- description: Unique cluster name.
  name: name
  type: string
- description: ''
  name: address
  type: object
- description: ''
  name: metadata
  type: object
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-cluster-node-schema.json
slug: rest-api-cluster-node
source_filename: rest-api-cluster-node-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-cluster-node-schema.json\",\n  \"title\": \"ClusterNode\",\n  \"description\": \"Information about the cluster node.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Node ID.\",\n      \"format\": \"uuid\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique cluster name.\"\n    },\n    \"address\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkAddress\"\n        },\n        {\n          \"description\": \"Cluster network address information.\"\n        }\n      ]\n    },\n    \"metadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeMetadata\"\n        },\n        {\n          \"description\": \"Node metadata information.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-cluster-node-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: ClusterNode
---
