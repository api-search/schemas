---
description: List of cluster shards
layout: schema
name: ShardList
properties_list:
- description: ''
  name: shards
  type: array
- description: Total shard count
  name: totalShards
  type: integer
- description: Total entities across all shards
  name: totalEntities
  type: integer
provider_name: Actor Model
provider_slug: actor-model
schema_file: json-schema/actor-model-shard-list-schema.json
slug: actor-model-shard-list
source_filename: actor-model-shard-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://schema.api-evangelist.com/actor-model/actor-model-shardlist-schema.json\",\n  \"title\": \"ShardList\",\n  \"description\": \"List of cluster shards\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"shards\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Shard\"\n      }\n    },\n    \"totalShards\": {\n      \"type\": \"integer\",\n      \"description\": \"Total shard count\",\n      \"example\": 100\n    },\n    \"totalEntities\": {\n      \"type\": \"integer\",\n      \"description\": \"Total entities across all shards\",\n      \"example\": 15000\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/actor-model/refs/heads/main/json-schema/actor-model-shard-list-schema.json
tags:
- Actor Model
- Concurrency
- Distributed Systems
title: ShardList
---
