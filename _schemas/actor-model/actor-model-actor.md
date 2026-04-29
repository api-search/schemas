---
description: An actor in the system with its current state and mailbox info
layout: schema
name: Actor
properties_list:
- description: Unique actor identifier
  name: id
  type: string
- description: Hierarchical actor path
  name: path
  type: string
- description: Current behavior class or name
  name: behavior
  type: string
- description: Current actor status
  name: status
  type: string
- description: Number of pending messages in mailbox
  name: mailboxSize
  type: integer
- description: Parent supervisor actor ID
  name: supervisorId
  type: string
- description: When the actor was spawned
  name: spawnedAt
  type: string
- description: Timestamp of last processed message
  name: lastMessageAt
  type: string
- description: Total messages processed since spawn
  name: messageCount
  type: integer
- description: Number of times this actor has been restarted
  name: restartCount
  type: integer
provider_name: Actor Model
provider_slug: actor-model
schema_file: json-schema/actor-model-actor-schema.json
slug: actor-model-actor
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://schema.api-evangelist.com/actor-model/actor-model-actor-schema.json\",\n  \"title\": \"Actor\",\n  \"description\": \"An actor in the system with its current state and mailbox info\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique actor identifier\",\n      \"example\": \"user-123\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"Hierarchical actor path\",\n      \"example\": \"/user/supervisor/worker-1\"\n    },\n    \"behavior\": {\n      \"type\": \"string\",\n      \"description\": \"Current behavior class or name\",\n      \"example\": \"UserSessionBehavior\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"active\",\n        \"idle\",\n        \"stopping\",\n        \"stopped\"\n      ],\n      \"description\": \"Current actor status\",\n     \
  \ \"example\": \"active\"\n    },\n    \"mailboxSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of pending messages in mailbox\",\n      \"example\": 3\n    },\n    \"supervisorId\": {\n      \"type\": \"string\",\n      \"description\": \"Parent supervisor actor ID\",\n      \"example\": \"supervisor-pool-1\"\n    },\n    \"spawnedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the actor was spawned\"\n    },\n    \"lastMessageAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of last processed message\"\n    },\n    \"messageCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total messages processed since spawn\",\n      \"example\": 1024\n    },\n    \"restartCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times this actor has been restarted\",\n      \"example\": 0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/actor-model/refs/heads/main/json-schema/actor-model-actor-schema.json
tags:
- Actor Model
- Concurrency
- Distributed Systems
title: Actor
---
