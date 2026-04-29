---
description: Cluster initialization configuration.
layout: schema
name: InitCommand
properties_list:
- description: A list of RAFT metastorage nodes.
  name: metaStorageNodes
  type: array
- description: A list of RAFT cluster management nodes.
  name: cmgNodes
  type: array
- description: The name of the cluster.
  name: clusterName
  type: string
- description: Cluster configuration in HOCON format.
  name: clusterConfiguration
  type: string
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-init-command-schema.json
slug: rest-api-init-command
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-init-command-schema.json\",\n  \"title\": \"InitCommand\",\n  \"description\": \"Cluster initialization configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metaStorageNodes\": {\n      \"type\": \"array\",\n      \"description\": \"A list of RAFT metastorage nodes.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"cmgNodes\": {\n      \"type\": \"array\",\n      \"description\": \"A list of RAFT cluster management nodes.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"clusterName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the cluster.\"\n    },\n    \"clusterConfiguration\": {\n      \"type\": \"string\",\n      \"description\": \"Cluster configuration in HOCON format.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-init-command-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: InitCommand
---
