---
description: Unique tag that identifies the cluster.
layout: schema
name: ClusterTag
properties_list:
- description: Unique cluster UUID. Generated automatically.
  name: clusterId
  type: string
- description: Unique cluster name.
  name: clusterName
  type: string
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-cluster-tag-schema.json
slug: rest-api-cluster-tag
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-cluster-tag-schema.json\",\n  \"title\": \"ClusterTag\",\n  \"description\": \"Unique tag that identifies the cluster.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clusterId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique cluster UUID. Generated automatically.\",\n      \"format\": \"uuid\"\n    },\n    \"clusterName\": {\n      \"type\": \"string\",\n      \"description\": \"Unique cluster name.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-cluster-tag-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: ClusterTag
---
