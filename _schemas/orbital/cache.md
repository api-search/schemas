---
description: Represents a cache configuration in Orbital, used for caching query results to improve performance. Orbital supports in-memory, Redis, and Hazelcast cache implementations.
layout: schema
name: Orbital Cache
properties_list:
- description: Name of the cache configuration.
  name: name
  type: string
- description: Cache implementation type.
  name: type
  type: string
- description: Current status of the cache.
  name: status
  type: string
provider_name: Orbital
provider_slug: orbital
schema_file: json-schema/cache.json
slug: cache
source_filename: cache.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/orbital/refs/heads/main/json-schema/cache.json\",\n  \"title\": \"Orbital Cache\",\n  \"description\": \"Represents a cache configuration in Orbital, used for caching query results to improve performance. Orbital supports in-memory, Redis, and Hazelcast cache implementations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the cache configuration.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Cache implementation type.\",\n      \"enum\": [\"IN_MEMORY\", \"REDIS\", \"HAZELCAST\"]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the cache.\",\n      \"enum\": [\"ACTIVE\", \"INACTIVE\"]\n    }\n  },\n  \"required\": [\"name\", \"type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/orbital/refs/heads/main/json-schema/cache.json
tags:
- Data
- Gateways
title: Orbital Cache
---
