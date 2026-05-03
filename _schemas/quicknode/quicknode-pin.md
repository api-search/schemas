---
description: Schema describing a QuickNode IPFS pin record.
layout: schema
name: QuickNode IPFS Pin
properties_list:
- description: Identifier of the pin request.
  name: requestId
  type: string
- description: Content identifier of the pinned object.
  name: cid
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: status
  type: string
- description: Size of pinned content in bytes.
  name: size
  type: integer
- description: ''
  name: createdAt
  type: string
provider_name: QuickNode
provider_slug: quicknode
schema_file: json-schema/quicknode-pin-schema.json
slug: quicknode-pin
source_filename: quicknode-pin-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/json-schema/quicknode-pin-schema.json\",\n  \"title\": \"QuickNode IPFS Pin\",\n  \"description\": \"Schema describing a QuickNode IPFS pin record.\",\n  \"type\": \"object\",\n  \"required\": [\"requestId\", \"cid\", \"status\"],\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the pin request.\"\n    },\n    \"cid\": {\n      \"type\": \"string\",\n      \"description\": \"Content identifier of the pinned object.\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"queued\", \"pinning\", \"pinned\", \"failed\"]\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"Size of pinned content in bytes.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/json-schema/quicknode-pin-schema.json
tags:
- Blockchain
- Web3
- Infrastructure
- RPC
- IPFS
- Streaming Data
- Webhooks
- Key-Value Store
title: QuickNode IPFS Pin
---
