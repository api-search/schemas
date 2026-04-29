---
description: Additional metadata for an asset transfer.
layout: schema
name: Transfer Metadata
properties_list:
- description: ISO 8601 timestamp of the block.
  name: blockTimestamp
  type: string
provider_name: Alchemy
provider_slug: alchemy
schema_file: json-schema/alchemy-transfers-api-transfer-metadata-schema.json
slug: alchemy-transfers-api-transfer-metadata
source_filename: alchemy-transfers-api-transfer-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/json-schema/alchemy-transfers-api-transfer-metadata-schema.json\",\n  \"title\": \"Transfer Metadata\",\n  \"description\": \"Additional metadata for an asset transfer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"blockTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the block.\",\n      \"example\": \"2026-04-19T10:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alchemy/refs/heads/main/json-schema/alchemy-transfers-api-transfer-metadata-schema.json
tags:
- Blockchain
- Cryptocurrency
- Web3
- Account Abstraction
- Ethereum
title: Transfer Metadata
---
