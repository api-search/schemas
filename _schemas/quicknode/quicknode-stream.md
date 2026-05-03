---
description: Schema describing a QuickNode Streams configuration.
layout: schema
name: QuickNode Stream
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: Blockchain network identifier (e.g. ethereum-mainnet, solana-mainnet).
  name: network
  type: string
- description: Dataset (e.g. blocks, transactions, logs).
  name: dataset
  type: string
- description: JavaScript or SQL filter expression applied to stream events.
  name: filter
  type: string
- description: ''
  name: destination
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: createdAt
  type: string
provider_name: QuickNode
provider_slug: quicknode
schema_file: json-schema/quicknode-stream-schema.json
slug: quicknode-stream
source_filename: quicknode-stream-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/json-schema/quicknode-stream-schema.json\",\n  \"title\": \"QuickNode Stream\",\n  \"description\": \"Schema describing a QuickNode Streams configuration.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"network\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"network\": {\n      \"type\": \"string\",\n      \"description\": \"Blockchain network identifier (e.g. ethereum-mainnet, solana-mainnet).\"\n    },\n    \"dataset\": {\n      \"type\": \"string\",\n      \"description\": \"Dataset (e.g. blocks, transactions, logs).\"\n    },\n    \"filter\": {\n      \"type\": \"string\",\n      \"description\": \"JavaScript or SQL filter expression applied to stream events.\"\n    },\n    \"destination\": {\n     \
  \ \"type\": \"string\",\n      \"enum\": [\"webhook\", \"postgres\", \"snowflake\", \"s3\"]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"pending\", \"active\", \"paused\", \"errored\", \"deleted\"]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/json-schema/quicknode-stream-schema.json
tags:
- Blockchain
- Web3
- Infrastructure
- RPC
- IPFS
- Streaming Data
- Webhooks
- Key-Value Store
title: QuickNode Stream
---
