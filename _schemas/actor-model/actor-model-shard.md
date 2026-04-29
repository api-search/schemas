---
description: A shard partition in the cluster
layout: schema
name: Shard
properties_list:
- description: Shard identifier
  name: shardId
  type: string
- description: Shard region name
  name: region
  type: string
- description: Node hosting this shard
  name: nodeId
  type: string
- description: Number of entities in this shard
  name: entityCount
  type: integer
- description: Shard status
  name: status
  type: string
provider_name: Actor Model
provider_slug: actor-model
schema_file: json-schema/actor-model-shard-schema.json
slug: actor-model-shard
source_filename: actor-model-shard-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://schema.api-evangelist.com/actor-model/actor-model-shard-schema.json\",\n  \"title\": \"Shard\",\n  \"description\": \"A shard partition in the cluster\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"shardId\": {\n      \"type\": \"string\",\n      \"description\": \"Shard identifier\",\n      \"example\": \"shard-42\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Shard region name\",\n      \"example\": \"UserRegion\"\n    },\n    \"nodeId\": {\n      \"type\": \"string\",\n      \"description\": \"Node hosting this shard\",\n      \"example\": \"akka://system@10.0.0.2:2551\"\n    },\n    \"entityCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of entities in this shard\",\n      \"example\": 150\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Shard status\",\n      \"example\": \"active\"\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/actor-model/refs/heads/main/json-schema/actor-model-shard-schema.json
tags:
- Actor Model
- Concurrency
- Distributed Systems
title: Shard
---
