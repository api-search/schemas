---
description: Schema for Redis XINFO STREAM response, providing detailed stream metadata.
layout: schema
name: Redis Stream Info
properties_list:
- description: Number of entries in the stream
  name: length
  type: integer
- description: Number of keys in the underlying radix tree
  name: radix-tree-keys
  type: integer
- description: Number of nodes in the underlying radix tree
  name: radix-tree-nodes
  type: integer
- description: The last generated ID (may not be the last entry ID if entries were deleted)
  name: last-generated-id
  type: string
- description: The maximum entry ID that was deleted from the stream
  name: max-deleted-entry-id
  type: string
- description: Total number of entries added to the stream over its lifetime
  name: entries-added
  type: integer
- description: The ID of the first entry in the stream
  name: recorded-first-entry-id
  type: string
- description: Number of consumer groups associated with the stream
  name: groups
  type: integer
- description: The first entry in the stream
  name: first-entry
  type: object
- description: The last entry in the stream
  name: last-entry
  type: object
provider_name: Redis Streams
provider_slug: redis-streams
schema_file: json-schema/redis-stream-info.json
slug: redis-stream-info
source_filename: redis-stream-info.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/redis-streams/redis-stream-info.json\",\n  \"title\": \"Redis Stream Info\",\n  \"description\": \"Schema for Redis XINFO STREAM response, providing detailed stream metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"length\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of entries in the stream\"\n    },\n    \"radix-tree-keys\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of keys in the underlying radix tree\"\n    },\n    \"radix-tree-nodes\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of nodes in the underlying radix tree\"\n    },\n    \"last-generated-id\": {\n      \"type\": \"string\",\n      \"description\": \"The last generated ID (may not be the last entry ID if entries were deleted)\"\n    },\n    \"max-deleted-entry-id\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The maximum entry ID that was deleted from the stream\"\n    },\n    \"entries-added\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of entries added to the stream over its lifetime\"\n    },\n    \"recorded-first-entry-id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the first entry in the stream\"\n    },\n    \"groups\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of consumer groups associated with the stream\"\n    },\n    \"first-entry\": {\n      \"type\": \"object\",\n      \"description\": \"The first entry in the stream\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"fields\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"last-entry\": {\n      \"type\": \"object\",\n      \"description\": \"The last entry in the stream\",\n      \"properties\"\
  : {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"fields\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/redis-streams/refs/heads/main/json-schema/redis-stream-info.json
tags:
- Consumer Groups
- Event-Driven
- In-Memory
- Messaging
- Redis
- Streaming
title: Redis Stream Info
---
