---
description: Schema for a key/value pair returned by the Consul KV API.
layout: schema
name: Consul KV Pair
properties_list:
- description: ''
  name: Key
  type: string
- description: Base64-encoded value of the key (null when not present).
  name: Value
  type:
  - string
  - 'null'
- description: User-defined 64-bit unsigned integer associated with the entry.
  name: Flags
  type: integer
- description: ''
  name: CreateIndex
  type: integer
- description: ''
  name: ModifyIndex
  type: integer
- description: ''
  name: LockIndex
  type: integer
- description: ID of the session holding the lock on this key, if any.
  name: Session
  type:
  - string
  - 'null'
- description: ''
  name: Namespace
  type: string
- description: ''
  name: Partition
  type: string
provider_name: HashiCorp Consul
provider_slug: consul
schema_file: json-schema/consul-kv-schema.json
slug: consul-kv
source_filename: consul-kv-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/consul/refs/heads/main/json-schema/consul-kv-schema.json\",\n  \"title\": \"Consul KV Pair\",\n  \"description\": \"Schema for a key/value pair returned by the Consul KV API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": { \"type\": \"string\" },\n    \"Value\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Base64-encoded value of the key (null when not present).\"\n    },\n    \"Flags\": {\n      \"type\": \"integer\",\n      \"description\": \"User-defined 64-bit unsigned integer associated with the entry.\"\n    },\n    \"CreateIndex\": { \"type\": \"integer\" },\n    \"ModifyIndex\": { \"type\": \"integer\" },\n    \"LockIndex\": { \"type\": \"integer\" },\n    \"Session\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the session holding the lock on this key, if any.\"\n    },\n\
  \    \"Namespace\": { \"type\": \"string\" },\n    \"Partition\": { \"type\": \"string\" }\n  },\n  \"required\": [\"Key\", \"CreateIndex\", \"ModifyIndex\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/consul/refs/heads/main/json-schema/consul-kv-schema.json
tags:
- ACL
- Configuration
- Health Checking
- Key/Value Store
- Multi-Datacenter
- Open Source
- Service Discovery
- Service Mesh
title: Consul KV Pair
---
