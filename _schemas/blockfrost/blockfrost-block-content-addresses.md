---
description: block_content_addresses schema from Blockfrost API
layout: schema
name: block_content_addresses
properties_list: []
provider_name: Blockfrost
provider_slug: blockfrost
schema_file: json-schema/blockfrost-block-content-addresses-schema.json
slug: blockfrost-block-content-addresses
source_filename: blockfrost-block-content-addresses-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/json-schema/blockfrost-block-content-addresses-schema.json\",\n  \"title\": \"block_content_addresses\",\n  \"description\": \"block_content_addresses schema from Blockfrost API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"address\": {\n        \"type\": \"string\",\n        \"description\": \"Address that was affected in the specified block\"\n      },\n      \"transactions\": {\n        \"type\": \"array\",\n        \"description\": \"List of transactions containing the address either in their inputs or outputs. Sorted by transaction index within a block, ascending.\",\n        \"items\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"tx_hash\": {\n              \"type\": \"string\"\n            }\n          },\n          \"required\"\
  : [\n            \"tx_hash\"\n          ]\n        }\n      }\n    },\n    \"required\": [\n      \"address\",\n      \"transactions\"\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/json-schema/blockfrost-block-content-addresses-schema.json
tags:
- Blockchain
- Cardano
- Cryptocurrency
- DApps
- NFT
- Web3
title: block_content_addresses
---
