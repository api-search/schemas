---
description: block_content_txs_cbor schema from Blockfrost API
layout: schema
name: block_content_txs_cbor
properties_list: []
provider_name: Blockfrost
provider_slug: blockfrost
schema_file: json-schema/blockfrost-block-content-txs-cbor-schema.json
slug: blockfrost-block-content-txs-cbor
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/json-schema/blockfrost-block-content-txs-cbor-schema.json\",\n  \"title\": \"block_content_txs_cbor\",\n  \"description\": \"block_content_txs_cbor schema from Blockfrost API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"tx_hash\": {\n        \"type\": \"string\",\n        \"description\": \"Hash of the transaction\"\n      },\n      \"cbor\": {\n        \"type\": \"string\",\n        \"description\": \"CBOR representation of the transaction data\"\n      }\n    },\n    \"required\": [\n      \"tx_hash\",\n      \"cbor\"\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/json-schema/blockfrost-block-content-txs-cbor-schema.json
tags:
- Blockchain
- Cardano
- Cryptocurrency
- DApps
- NFT
- Web3
title: block_content_txs_cbor
---
