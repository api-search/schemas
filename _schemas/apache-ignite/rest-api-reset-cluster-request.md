---
description: Reset cluster.
layout: schema
name: ResetClusterRequest
properties_list:
- description: Names of the proposed CMG nodes. Optional if the MG group is being repaired. If not specified, the current CMG nodes are used.
  name: cmgNodeNames
  type: array
- description: Number of nodes in the voting member set of the Metastorage RAFT group.
  name: metastorageReplicationFactor
  type: integer
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-reset-cluster-request-schema.json
slug: rest-api-reset-cluster-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-reset-cluster-request-schema.json\",\n  \"title\": \"ResetClusterRequest\",\n  \"description\": \"Reset cluster.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cmgNodeNames\": {\n      \"type\": \"array\",\n      \"description\": \"Names of the proposed CMG nodes. Optional if the MG group is being repaired. If not specified, the current CMG nodes are used.\",\n      \"nullable\": true,\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"metastorageReplicationFactor\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of nodes in the voting member set of the Metastorage RAFT group.\",\n      \"format\": \"int32\",\n      \"nullable\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-reset-cluster-request-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: ResetClusterRequest
---
