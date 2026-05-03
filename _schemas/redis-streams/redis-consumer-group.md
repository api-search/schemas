---
description: Schema for a Redis Streams consumer group configuration and state.
layout: schema
name: Redis Streams Consumer Group
properties_list:
- description: The consumer group name
  name: name
  type: string
- description: The stream key this consumer group is attached to
  name: stream
  type: string
- description: The ID of the last entry delivered to the group
  name: last-delivered-id
  type: string
- description: Total number of entries read by the group (Redis 7.0+)
  name: entries-read
  type: integer
- description: Number of entries in the stream that are still waiting to be delivered (Redis 7.0+)
  name: lag
  type: integer
- description: Number of entries in the Pending Entries List (PEL)
  name: pel-count
  type: integer
- description: List of consumers in this group
  name: consumers
  type: array
provider_name: Redis Streams
provider_slug: redis-streams
schema_file: json-schema/redis-consumer-group.json
slug: redis-consumer-group
source_filename: redis-consumer-group.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/redis-streams/redis-consumer-group.json\",\n  \"title\": \"Redis Streams Consumer Group\",\n  \"description\": \"Schema for a Redis Streams consumer group configuration and state.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The consumer group name\"\n    },\n    \"stream\": {\n      \"type\": \"string\",\n      \"description\": \"The stream key this consumer group is attached to\"\n    },\n    \"last-delivered-id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the last entry delivered to the group\"\n    },\n    \"entries-read\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of entries read by the group (Redis 7.0+)\"\n    },\n    \"lag\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of entries in the stream that are\
  \ still waiting to be delivered (Redis 7.0+)\"\n    },\n    \"pel-count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of entries in the Pending Entries List (PEL)\"\n    },\n    \"consumers\": {\n      \"type\": \"array\",\n      \"description\": \"List of consumers in this group\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Consumer name\"\n          },\n          \"pending\": {\n            \"type\": \"integer\",\n            \"description\": \"Number of pending entries for this consumer\"\n          },\n          \"idle\": {\n            \"type\": \"integer\",\n            \"description\": \"Idle time in milliseconds since last interaction\"\n          },\n          \"inactive\": {\n            \"type\": \"integer\",\n            \"description\": \"Inactive time in milliseconds (Redis 7.2+)\"\n          }\n        }\n      }\n    }\n  },\n\
  \  \"required\": [\"name\", \"stream\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/redis-streams/refs/heads/main/json-schema/redis-consumer-group.json
tags:
- Consumer Groups
- Event-Driven
- In-Memory
- Messaging
- Redis
- Streaming
title: Redis Streams Consumer Group
---
