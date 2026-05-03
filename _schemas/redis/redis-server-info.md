---
description: Key metrics from the Redis INFO command, covering server, clients, memory, persistence, replication, and stats sections.
layout: schema
name: Redis Server Info
properties_list:
- description: Redis server version string (e.g., 7.2.0).
  name: redis_version
  type: string
- description: Redis operational mode.
  name: redis_mode
  type: string
- description: Number of seconds since server start.
  name: uptime_in_seconds
  type: integer
- description: Number of client connections (excluding replica connections).
  name: connected_clients
  type: integer
- description: Total bytes allocated by Redis using its allocator.
  name: used_memory
  type: integer
- description: Human-readable used memory (e.g., 1.23M).
  name: used_memory_human
  type: string
- description: Maximum memory configured. 0 means no limit.
  name: maxmemory
  type: integer
- description: Eviction policy when maxmemory is reached.
  name: maxmemory_policy
  type: string
- description: Unix timestamp of last successful RDB save.
  name: rdb_last_save_time
  type: integer
- description: Whether AOF persistence is enabled (1) or disabled (0).
  name: aof_enabled
  type: integer
- description: Replication role of this instance.
  name: role
  type: string
- description: Number of connected replicas.
  name: connected_slaves
  type: integer
- description: Total number of commands processed since server start.
  name: total_commands_processed
  type: integer
- description: Total connections accepted since server start.
  name: total_connections_received
  type: integer
- description: Number of successful key lookups.
  name: keyspace_hits
  type: integer
- description: Number of failed key lookups.
  name: keyspace_misses
  type: integer
- description: Total number of key expiration events.
  name: expired_keys
  type: integer
- description: Number of keys evicted due to maxmemory policy.
  name: evicted_keys
  type: integer
- description: Per-database key statistics.
  name: db
  type: object
provider_name: Redis
provider_slug: redis
schema_file: json-schema/redis-server-info-schema.json
slug: redis-server-info
source_filename: redis-server-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://redis.io/schemas/server-info.json\",\n  \"title\": \"Redis Server Info\",\n  \"description\": \"Key metrics from the Redis INFO command, covering server, clients, memory, persistence, replication, and stats sections.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"redis_version\": {\n      \"type\": \"string\",\n      \"description\": \"Redis server version string (e.g., 7.2.0).\"\n    },\n    \"redis_mode\": {\n      \"type\": \"string\",\n      \"enum\": [\"standalone\", \"sentinel\", \"cluster\"],\n      \"description\": \"Redis operational mode.\"\n    },\n    \"uptime_in_seconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of seconds since server start.\"\n    },\n    \"connected_clients\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of client connections (excluding replica connections).\"\n    },\n    \"used_memory\": {\n      \"\
  type\": \"integer\",\n      \"description\": \"Total bytes allocated by Redis using its allocator.\"\n    },\n    \"used_memory_human\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable used memory (e.g., 1.23M).\"\n    },\n    \"maxmemory\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum memory configured. 0 means no limit.\"\n    },\n    \"maxmemory_policy\": {\n      \"type\": \"string\",\n      \"enum\": [\"noeviction\", \"allkeys-lru\", \"volatile-lru\", \"allkeys-random\", \"volatile-random\", \"volatile-ttl\", \"allkeys-lfu\", \"volatile-lfu\"],\n      \"description\": \"Eviction policy when maxmemory is reached.\"\n    },\n    \"rdb_last_save_time\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of last successful RDB save.\"\n    },\n    \"aof_enabled\": {\n      \"type\": \"integer\",\n      \"enum\": [0, 1],\n      \"description\": \"Whether AOF persistence is enabled (1) or disabled (0).\"\n    },\n    \"\
  role\": {\n      \"type\": \"string\",\n      \"enum\": [\"master\", \"replica\", \"slave\"],\n      \"description\": \"Replication role of this instance.\"\n    },\n    \"connected_slaves\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of connected replicas.\"\n    },\n    \"total_commands_processed\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of commands processed since server start.\"\n    },\n    \"total_connections_received\": {\n      \"type\": \"integer\",\n      \"description\": \"Total connections accepted since server start.\"\n    },\n    \"keyspace_hits\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of successful key lookups.\"\n    },\n    \"keyspace_misses\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of failed key lookups.\"\n    },\n    \"expired_keys\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of key expiration events.\"\n    },\n    \"evicted_keys\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Number of keys evicted due to maxmemory policy.\"\n    },\n    \"db\": {\n      \"type\": \"object\",\n      \"description\": \"Per-database key statistics.\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"keys\": { \"type\": \"integer\" },\n          \"expires\": { \"type\": \"integer\" },\n          \"avg_ttl\": { \"type\": \"integer\" }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/redis/refs/heads/main/json-schema/redis-server-info-schema.json
tags:
- Cache
- Database
- In-Memory
- Key-Value Store
- NoSQL
- Open Source
- Streaming
title: Redis Server Info
---
