---
description: Schema for a Redis Streams entry, consisting of an auto-generated ID and field-value pairs.
layout: schema
name: Redis Stream Entry
properties_list:
- description: Stream entry ID in format <millisecondsTime>-<sequenceNumber>, e.g., 1526919030474-55. Can be auto-generated with *.
  name: id
  type: string
- description: Key-value pairs forming the stream entry data. Redis stores all values as strings.
  name: fields
  type: object
provider_name: Redis Streams
provider_slug: redis-streams
schema_file: json-schema/redis-stream-entry.json
slug: redis-stream-entry
source_filename: redis-stream-entry.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/redis-streams/redis-stream-entry.json\",\n  \"title\": \"Redis Stream Entry\",\n  \"description\": \"Schema for a Redis Streams entry, consisting of an auto-generated ID and field-value pairs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[0-9]+-[0-9]+$\",\n      \"description\": \"Stream entry ID in format <millisecondsTime>-<sequenceNumber>, e.g., 1526919030474-55. Can be auto-generated with *.\"\n    },\n    \"fields\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Key-value pairs forming the stream entry data. Redis stores all values as strings.\"\n    }\n  },\n  \"required\": [\"fields\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/redis-streams/refs/heads/main/json-schema/redis-stream-entry.json
tags:
- Consumer Groups
- Event-Driven
- In-Memory
- Messaging
- Redis
- Streaming
title: Redis Stream Entry
---
