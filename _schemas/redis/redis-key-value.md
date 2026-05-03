---
description: A Redis key and its associated value, type, and metadata.
layout: schema
name: Redis Key-Value Entry
properties_list:
- description: The Redis key. Keys are arbitrary binary-safe strings, conventionally namespaced with colons (e.g., user:1234:profile).
  name: key
  type: string
- description: The Redis data type for this key.
  name: type
  type: string
- description: The value stored at this key. Type depends on the Redis data type.
  name: value
  type: object
- description: Time-to-live in seconds. -1 means no expiry. -2 means the key does not exist.
  name: ttl
  type: integer
- description: Internal Redis encoding for the value (e.g., embstr, raw, ziplist, listpack, skiplist, quicklist, hashtable).
  name: encoding
  type: string
provider_name: Redis
provider_slug: redis
schema_file: json-schema/redis-key-value-schema.json
slug: redis-key-value
source_filename: redis-key-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://redis.io/schemas/key-value.json\",\n  \"title\": \"Redis Key-Value Entry\",\n  \"description\": \"A Redis key and its associated value, type, and metadata.\",\n  \"type\": \"object\",\n  \"required\": [\"key\"],\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The Redis key. Keys are arbitrary binary-safe strings, conventionally namespaced with colons (e.g., user:1234:profile).\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"string\", \"list\", \"set\", \"zset\", \"hash\", \"stream\", \"json\", \"none\"],\n      \"description\": \"The Redis data type for this key.\"\n    },\n    \"value\": {\n      \"description\": \"The value stored at this key. Type depends on the Redis data type.\",\n      \"oneOf\": [\n        { \"type\": \"string\", \"description\": \"String value.\" },\n        { \"type\": \"array\", \"description\"\
  : \"List or set value.\", \"items\": { \"type\": \"string\" } },\n        { \"type\": \"object\", \"description\": \"Hash or JSON value.\" }\n      ]\n    },\n    \"ttl\": {\n      \"type\": \"integer\",\n      \"description\": \"Time-to-live in seconds. -1 means no expiry. -2 means the key does not exist.\",\n      \"minimum\": -2\n    },\n    \"encoding\": {\n      \"type\": \"string\",\n      \"description\": \"Internal Redis encoding for the value (e.g., embstr, raw, ziplist, listpack, skiplist, quicklist, hashtable).\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/redis/refs/heads/main/json-schema/redis-key-value-schema.json
tags:
- Cache
- Database
- In-Memory
- Key-Value Store
- NoSQL
- Open Source
- Streaming
title: Redis Key-Value Entry
---
