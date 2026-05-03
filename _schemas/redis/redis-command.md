---
description: Schema for a Redis command descriptor as returned by the COMMAND INFO command.
layout: schema
name: Redis Command
properties_list:
- description: Command name in lowercase (e.g., get, set, hset).
  name: name
  type: string
- description: 'Command arity: number of required arguments. Negative arity means minimum argument count (e.g., -2 means at least 1 arg after command name).'
  name: arity
  type: integer
- description: Command flags indicating behavior (e.g., write, readonly, denyoom, admin).
  name: flags
  type: array
- description: Index of first key in argument list.
  name: first_key
  type: integer
- description: Index of last key in argument list. -1 means last argument.
  name: last_key
  type: integer
- description: Step between keys in argument list.
  name: step
  type: integer
- description: ACL categories the command belongs to.
  name: acl_categories
  type: array
- description: Time complexity annotation (e.g., O(1), O(N), O(log N)).
  name: complexity
  type: string
provider_name: Redis
provider_slug: redis
schema_file: json-schema/redis-command-schema.json
slug: redis-command
source_filename: redis-command-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://redis.io/schemas/command.json\",\n  \"title\": \"Redis Command\",\n  \"description\": \"Schema for a Redis command descriptor as returned by the COMMAND INFO command.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"arity\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Command name in lowercase (e.g., get, set, hset).\"\n    },\n    \"arity\": {\n      \"type\": \"integer\",\n      \"description\": \"Command arity: number of required arguments. Negative arity means minimum argument count (e.g., -2 means at least 1 arg after command name).\"\n    },\n    \"flags\": {\n      \"type\": \"array\",\n      \"description\": \"Command flags indicating behavior (e.g., write, readonly, denyoom, admin).\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"write\", \"readonly\", \"denyoom\", \"admin\", \"pubsub\", \"\
  noscript\", \"random\", \"sort_for_script\", \"loading\", \"stale\", \"skip_monitor\", \"asking\", \"fast\", \"no_auth\", \"may_replicate\", \"sentinel\", \"only_sentinel\", \"allow_busy\", \"module_getkeys\"]\n      }\n    },\n    \"first_key\": {\n      \"type\": \"integer\",\n      \"description\": \"Index of first key in argument list.\"\n    },\n    \"last_key\": {\n      \"type\": \"integer\",\n      \"description\": \"Index of last key in argument list. -1 means last argument.\"\n    },\n    \"step\": {\n      \"type\": \"integer\",\n      \"description\": \"Step between keys in argument list.\"\n    },\n    \"acl_categories\": {\n      \"type\": \"array\",\n      \"description\": \"ACL categories the command belongs to.\",\n      \"items\": { \"type\": \"string\" }\n    },\n    \"complexity\": {\n      \"type\": \"string\",\n      \"description\": \"Time complexity annotation (e.g., O(1), O(N), O(log N)).\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/redis/refs/heads/main/json-schema/redis-command-schema.json
tags:
- Cache
- Database
- In-Memory
- Key-Value Store
- NoSQL
- Open Source
- Streaming
title: Redis Command
---
