---
description: List of cluster members
layout: schema
name: ClusterMemberList
properties_list:
- description: ''
  name: members
  type: array
- description: Current cluster leader node ID
  name: leader
  type: string
- description: Total actors across all cluster members
  name: totalActors
  type: integer
provider_name: Actor Model
provider_slug: actor-model
schema_file: json-schema/actor-model-cluster-member-list-schema.json
slug: actor-model-cluster-member-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://schema.api-evangelist.com/actor-model/actor-model-clustermemberlist-schema.json\",\n  \"title\": \"ClusterMemberList\",\n  \"description\": \"List of cluster members\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"members\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ClusterMember\"\n      }\n    },\n    \"leader\": {\n      \"type\": \"string\",\n      \"description\": \"Current cluster leader node ID\",\n      \"example\": \"akka://system@10.0.0.1:2551\"\n    },\n    \"totalActors\": {\n      \"type\": \"integer\",\n      \"description\": \"Total actors across all cluster members\",\n      \"example\": 5000\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/actor-model/refs/heads/main/json-schema/actor-model-cluster-member-list-schema.json
tags:
- Actor Model
- Concurrency
- Distributed Systems
title: ClusterMemberList
---
