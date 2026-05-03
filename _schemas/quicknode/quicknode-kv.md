---
description: Schema describing a QuickNode Key-Value Store record.
layout: schema
name: QuickNode Key-Value Record
properties_list:
- description: Name of the key-value database.
  name: database
  type: string
- description: ''
  name: key
  type: string
- description: ''
  name: value
  type:
  - string
  - number
  - boolean
  - object
  - array
  - 'null'
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: QuickNode
provider_slug: quicknode
schema_file: json-schema/quicknode-kv-schema.json
slug: quicknode-kv
source_filename: quicknode-kv-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/json-schema/quicknode-kv-schema.json\",\n  \"title\": \"QuickNode Key-Value Record\",\n  \"description\": \"Schema describing a QuickNode Key-Value Store record.\",\n  \"type\": \"object\",\n  \"required\": [\"database\", \"key\"],\n  \"properties\": {\n    \"database\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the key-value database.\"\n    },\n    \"key\": {\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"type\": [\"string\", \"number\", \"boolean\", \"object\", \"array\", \"null\"]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/json-schema/quicknode-kv-schema.json
tags:
- Blockchain
- Web3
- Infrastructure
- RPC
- IPFS
- Streaming Data
- Webhooks
- Key-Value Store
title: QuickNode Key-Value Record
---
