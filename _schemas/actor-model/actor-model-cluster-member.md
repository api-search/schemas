---
description: A node in the actor system cluster
layout: schema
name: ClusterMember
properties_list:
- description: Unique node identifier
  name: nodeId
  type: string
- description: Network address
  name: address
  type: string
- description: Member status
  name: status
  type: string
- description: Node roles
  name: roles
  type: array
- description: When node joined the cluster
  name: upSince
  type: string
- description: Number of actors hosted on this node
  name: actorCount
  type: integer
provider_name: Actor Model
provider_slug: actor-model
schema_file: json-schema/actor-model-cluster-member-schema.json
slug: actor-model-cluster-member
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://schema.api-evangelist.com/actor-model/actor-model-clustermember-schema.json\",\n  \"title\": \"ClusterMember\",\n  \"description\": \"A node in the actor system cluster\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nodeId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique node identifier\",\n      \"example\": \"akka://system@10.0.0.1:2551\"\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Network address\",\n      \"example\": \"10.0.0.1:2551\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"up\",\n        \"joining\",\n        \"leaving\",\n        \"down\",\n        \"removed\"\n      ],\n      \"description\": \"Member status\",\n      \"example\": \"up\"\n    },\n    \"roles\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"\
  Node roles\",\n      \"example\": [\n        \"worker\",\n        \"seed\"\n      ]\n    },\n    \"upSince\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When node joined the cluster\"\n    },\n    \"actorCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of actors hosted on this node\",\n      \"example\": 1200\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/actor-model/refs/heads/main/json-schema/actor-model-cluster-member-schema.json
tags:
- Actor Model
- Concurrency
- Distributed Systems
title: ClusterMember
---
